# ConsertaTech Mobile — App

Área responsável pelo aplicativo Android em Kotlin.

## Responsabilidades

- telas e navegação;
- componentes de interface;
- integração com a API REST;
- gerenciamento de estado local;
- validações de entrada;
- armazenamento local somente quando necessário e de forma segura;
- experiência do usuário em dispositivos móveis.

A implementação deve seguir as regras de negócio documentadas e consumir o back-end, evitando acesso direto ao banco de dados para operações sensíveis.

## Estrutura prevista

```text
mobile/
├── src/
│   ├── main/
│   ├── test/
│   └── androidTest/
├── assets/
└── README.md
```

A arquitetura interna do aplicativo será definida antes do início da implementação das telas.