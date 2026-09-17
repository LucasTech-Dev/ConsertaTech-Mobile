# Back-end Kotlin

Área responsável pela API e pelas regras de negócio utilizadas pelo aplicativo.

## Tecnologia

- Kotlin
- API REST
- Integração com o mesmo banco de dados do ConsertaTech Web

## Estrutura prevista

```text
backend/src/main/kotlin/
├── controllers/
├── middlewares/
├── models/
├── routes/
├── services/
└── utils/
```

O framework de servidor Kotlin será definido pela equipe antes da implementação da API. O back-end deve concentrar autenticação, autorização, regras de negócio, validações, acesso ao banco e tratamento de erros.

Nunca colocar credenciais do banco ou outros segredos no aplicativo ou no repositório.