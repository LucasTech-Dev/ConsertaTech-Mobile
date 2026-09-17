# Fluxo Git da equipe

## Branches individuais

```text
dev/lucas
dev/arthur
dev/emanuele
dev/murilo
dev/paulo
dev/benjamin
dev/gabriel
```

Cada integrante trabalha em sua própria branch.

## Branches de integração

```text
pre-main/mobile
pre-main/backend
mobile-main
back-main
main
```

## Fluxo

```text
dev/<pessoa>
      ↓
Pull Request
      ↓
pre-main/mobile ou pre-main/backend
      ↓
revisão + testes
      ↓
mobile-main ou back-main
      ↓
integração
      ↓
main
```

## Regras

- Não desenvolver diretamente na `main`.
- Commits devem descrever claramente a alteração.
- Pull Requests devem explicar o que foi alterado e como testar.
- Mudanças que afetam API ou banco devem ser comunicadas/documentadas.
- Antes de integrar, verificar se a alteração não quebra o outro lado do sistema.
