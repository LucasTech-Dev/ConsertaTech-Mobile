# ConsertaTech Mobile

Versão mobile do ConsertaTech, desenvolvida em paralelo ao sistema Web.

## Objetivo

Disponibilizar no ambiente mobile as funcionalidades do ConsertaTech para técnicos, pequenas assistências técnicas e clientes, mantendo as mesmas regras de negócio e integração com o ecossistema existente.

## Relação com o projeto Web

Este repositório é separado do `ConsertaTech` Web, mas faz parte do mesmo produto. A intenção é reutilizar conceitos, regras de negócio, identidade visual e o mesmo banco de dados, adaptando somente o necessário para o ambiente mobile.

## Stack

| Área | Tecnologia |
|---|---|
| Aplicativo | Kotlin / Android |
| Back-end | Kotlin |
| API | REST |
| Banco de dados | Mesmo banco do ConsertaTech Web |
| Controle de versão | Git + GitHub |
| IDE recomendada | Android Studio para o app / IDE compatível com Kotlin para o back-end |

> O framework específico do back-end Kotlin será definido antes da implementação da API. Não deve ser escolhido ou adicionado sem decisão da equipe.

## Estrutura

```text
ConsertaTech-Mobile/
├── mobile/
│   ├── src/
│   ├── assets/
│   └── README.md
├── backend/
│   ├── src/
│   │   └── main/
│   │       ├── kotlin/
│   │       └── resources/
│   └── README.md
├── database/
│   ├── schema/
│   ├── migrations/
│   ├── seeds/
│   ├── backups/
│   └── README.md
├── security/
│   ├── policies/
│   ├── checklists/
│   └── README.md
├── design/
│   ├── brand/
│   ├── prototypes/
│   └── README.md
├── docs/
│   ├── ARCHITECTURE.md
│   └── GIT-FLOW.md
├── .gitignore
└── README.md
```

## Equipe

A mesma equipe do projeto Web trabalha neste repositório em todas as áreas:

- Lucas
- Arthur
- Emanuele
- Murilo
- Paulo
- Benjamin
- Gabriel

## Fluxo Git

```text
dev/<desenvolvedor>
        ↓
pre-main/mobile ou pre-main/backend
        ↓
mobile-main ou back-main
        ↓
main
```

- `dev/*`: desenvolvimento individual.
- `pre-main/mobile`: integração, revisão e testes do aplicativo.
- `pre-main/backend`: integração, revisão e testes do back-end Kotlin.
- `mobile-main`: versão mobile pronta para integração.
- `back-main`: versão do back-end pronta para integração.
- `main`: versão integrada e funcional.

Não trabalhar diretamente na `main`. Alterações devem passar pelo fluxo de branches e Pull Requests.

## Banco de dados

O aplicativo não cria um banco independente. O projeto utiliza o mesmo banco definido para o ConsertaTech Web. Credenciais e segredos nunca devem ser armazenados no código ou no GitHub.

## Regras de segurança

- Não armazenar senhas, tokens, chaves ou credenciais no repositório.
- Não colocar credenciais de banco no aplicativo mobile.
- Operações sensíveis devem passar pelo back-end.
- Validar dados no cliente e, principalmente, no servidor.
- Documentar mudanças de segurança.

## Critério inicial de pronto

Outro integrante deve conseguir clonar o repositório, identificar sua área de trabalho e entender o fluxo de contribuição somente pela documentação deste repositório.