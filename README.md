
# 📋 WA Suite CRM

Um mini-CRM web estilo Bitrix24, 100% responsivo, com painel Kanban, autenticação local e integração com Firebase Firestore.

## 🔥 Funcionalidades

- Login com email/senha (simulado via localStorage ou integrado com Firebase UID)
- Painel Kanban com 4 etapas: Leads, Contato, Negociação, Fechado
- Criação, edição e remoção de clientes
- Campo de agendamento com notificação de vencimento
- Gráfico de clientes por etapa (Chart.js)
- Lista dos últimos 5 clientes adicionados
- Filtro por data (ex: últimos 7 dias)
- Layout adaptado para desktop e mobile

## 🧪 Acesso de exemplo

```
Email: admin@wasuite.com
Senha: 123456

ou

Email: thiago@mobileon.com
Senha: mobileon
```

## 🚀 Como usar no GitHub Pages

1. Faça upload dos arquivos `index.html` e `dashboard.html` para o seu repositório
2. Vá em **Settings > Pages**
3. Em **Source**, selecione `main branch` e pasta `/root`
4. Acesse: `https://seuusuario.github.io/seurepositorio`

## 🔗 Integração com Firebase

- Firestore usado para armazenar os cards
- Cada card contém:
```js
{
  uid: "ID do usuário",
  nome: "Cliente",
  telefone: "Contato",
  comentario: "Notas",
  etapa: "leads | contato | negociacao | fechado",
  agendamento: "YYYY-MM-DD HH:mm"
}
```

## 📦 Estrutura de arquivos

| Arquivo         | Função                               |
|-----------------|--------------------------------------|
| `index.html`    | Tela de login                        |
| `dashboard.html`| Painel Kanban e funcionalidades CRM  |
| `README.md`     | Instruções e documentação            |

## 📍 To-Do futuro

- [ ] Backend com autenticação Firebase real
- [ ] Criação de usuários via interface
- [ ] Integração com envio de mensagens (ex: WhatsApp API)
- [ ] Relatórios PDF e exportação Excel
