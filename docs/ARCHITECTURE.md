# Arquitetura — ConsertaTech Mobile

## Visão geral

O Mobile é um cliente do ecossistema ConsertaTech. O aplicativo conversa com o back-end por API REST e o back-end acessa o mesmo banco de dados utilizado pelo produto Web.

```text
┌─────────────────────┐
│ ConsertaTech Mobile │
│ Kotlin / Android    │
└──────────┬──────────┘
           │ REST API
           ▼
┌─────────────────────┐
│ Back-end Kotlin     │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Banco compartilhado │
│ com o projeto Web   │
└─────────────────────┘
```

## Princípios

1. Web e Mobile devem respeitar as mesmas regras de negócio.
2. O banco continua compartilhado.
3. O aplicativo não deve conter credenciais do banco.
4. O back-end é responsável pelas operações sensíveis.
5. Contratos da API devem ser documentados para permitir evolução coordenada.
6. Mudanças no banco devem considerar os dois clientes.

## Adaptação

Não copiar a interface Web para o Mobile. Reutilizar conceitos, fluxos, dados e identidade visual, redesenhando a interação para Android.