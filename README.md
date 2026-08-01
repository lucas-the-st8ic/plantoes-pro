# 🏥 Plantões & Folgas Pro

Aplicativo web para gerenciamento de plantões, folgas, feriados e eventos pessoais — sincronizado em tempo real entre todos os seus dispositivos.

🔗 **[Acessar o app](https://lucas-the-st8ic.github.io/plantoes-pro/)**

> Versão atual: **v1.1**

---

## ✨ Funcionalidades

- 📅 **Calendário anual completo** — visualize todos os 12 meses de uma vez
- 🗓 **Mês atual em destaque** — calendário maior com painel lateral de resumo e eventos do mês
- ⬛ **Faixa diagonal nos plantões** — identificação visual rápida dos dias de trabalho
- 🎨 **Cores personalizáveis** — escolha a cor de cada tipo de dia com paleta, swatches ou código hex
- 🔄 **Plantões automáticos** — marque o ano todo com um clique (dia sim/dia não e outros padrões)
- 📌 **Eventos e compromissos** — adicione eventos com nome, descrição, emoji e cor; visualize no calendário e em lista
- 📋 **Histórico de alterações** — registro de tudo que foi adicionado, editado ou removido, com data e hora
- ☁️ **Sincronização em tempo real** — Firebase salva e sincroniza entre celular, tablet e computador instantaneamente
- 🔐 **Login com Google** — dados isolados por conta, sem mistura entre usuários
- ⬇️ **Exportação CSV** — abra seus plantões e eventos no Excel ou Google Sheets
- 🌙 **Modo escuro** — interface escura por padrão, confortável para uso noturno
- 📱 **Responsivo** — funciona em qualquer tamanho de tela, celular ou desktop

---

## 🗂️ Tipos de dia

| Tipo | Descrição |
|------|-----------|
| ⬛ **Plantão** | Dia de trabalho — fundo colorido com faixa diagonal característica |
| 🟢 **Folga fixa** | Folga regular da escala |
| 🟠 **Folga adicional** | Folga extra ou trocada |
| 🟡 **Feriado** | Feriados nacionais (pré-carregados automaticamente) |
| 🟣 **Ponto facultativo** | Pontos facultativos nacionais (pré-carregados automaticamente) |

---

## 📌 Sistema de Eventos

Adicione compromissos e eventos a qualquer dia do calendário:

- **Nome** do evento e **descrição** opcional
- **Emoji personalizado** — digite ou cole qualquer emoji diretamente
- **Cor** — escolha entre 10 cores para identificar visualmente o evento
- Os eventos aparecem como bolinhas coloridas ou emojis abaixo do número do dia
- Clique no evento para expandir e ver todos os detalhes, editar ou excluir
- Eventos do mês atual listados no painel lateral do mês em destaque
- Eventos incluídos na exportação CSV

---

## 🗓️ Mês em Destaque

O mês atual aparece em destaque no topo da página com:

- **Calendário ampliado** à esquerda com dias espaçados e bordas discretas
- **Painel lateral** à direita com:
  - Contagem de plantões, folgas fixas, folgas adicionais e feriados do mês
  - Lista de todos os eventos do mês em ordem de data

---

## 📅 Feriados incluídos automaticamente

- Confraternização Universal (01/01)
- Sexta-Feira Santa (data variável)
- Tiradentes (21/04)
- Dia do Trabalho (01/05)
- Independência do Brasil (07/09)
- Nossa Sra. Aparecida (12/10)
- Finados (02/11)
- Proclamação da República (15/11)
- Consciência Negra (20/11)
- Natal (25/12)
- Carnaval e Corpus Christi (pontos facultativos)

---

## ⚙️ Plantões automáticos

Marque o ano inteiro de uma vez escolhendo o padrão de escala:

| Padrão | Descrição |
|--------|-----------|
| 1×1 | Dia sim, dia não |
| 2×1 | 2 plantões, 1 folga |
| 2×2 | 2 plantões, 2 folgas |
| 3×3 | 3 plantões, 3 folgas |
| 6×6 | 6 plantões, 6 folgas |

Dias já marcados não são sobrescritos. A folga pode ser marcada como fixa, adicional ou ignorada.

---

## 🚀 Como usar

1. Acesse **[https://lucas-the-st8ic.github.io/plantoes-pro/](https://lucas-the-st8ic.github.io/plantoes-pro/)**
2. Clique em **Entrar com Google**
3. Clique em qualquer dia para marcar plantão, folga ou adicionar um evento
4. Use **⚙ Automático** para marcar o ano todo de uma vez
5. Use **🎨 Cores** para personalizar as cores de cada tipo de dia
6. Use **＋ Evento** para adicionar compromissos e eventos ao calendário

### Adicionar à tela inicial (mobile)

- **iPhone/iPad:** Safari → Compartilhar → "Adicionar à Tela de Início"
- **Android:** Chrome → Menu (⋮) → "Adicionar à tela inicial"

---

## 🔧 Tecnologias

- **HTML / CSS / JavaScript** — sem frameworks, arquivo único
- **Firebase Authentication** — login com Google
- **Firebase Realtime Database** — sincronização em tempo real de dias, eventos, cores e histórico
- **GitHub Pages** — hospedagem gratuita

---

## 📦 Estrutura de dados no Firebase

```
users/
  {uid}/
    days/       → plantões e folgas marcados
    events/     → eventos e compromissos
    colors/     → cores personalizadas
    history/    → histórico de alterações (últimas 50)
```

---

## 🔒 Privacidade

Cada usuário tem seus dados completamente isolados no Firebase. Nenhuma conta tem acesso aos dados de outra. O app não coleta nem compartilha informações com terceiros.

---

## 📝 Changelog

### v1.1
- Adicionado **mês atual em destaque** com layout dois painéis (calendário + resumo e eventos)
- Adicionado **sistema de eventos** com emoji, cor, nome e descrição
- Eventos visíveis no calendário como bolinhas ou emojis abaixo do número do dia
- Modal expandido ao clicar no evento com todos os detalhes
- Histórico de alterações salvo no Firebase com data e hora
- Melhoria no visual dos dias com bordas e espaçamento mais confortáveis
- CSV atualizado com coluna de eventos

### v1.0
- Calendário anual completo com 12 meses
- Login com Google via Firebase
- Sincronização em tempo real entre dispositivos
- Plantões automáticos por padrão de escala
- Cores personalizáveis por tipo de dia
- Faixa diagonal nos dias de plantão
- Feriados e pontos facultativos pré-carregados
- Exportação para CSV

---

*Desenvolvido para uso pessoal. Sincronizado com Firebase.*