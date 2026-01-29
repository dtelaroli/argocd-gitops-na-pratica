# Exemplos do ebook (Volume I)

Este diretorio reune os exemplos apresentados no Volume I em formato de arquivos.

## Capitulo 5
- `examples/volume-I/cap-05/05-application.yaml` — exemplo completo de Application.

## Capitulo 9
- `examples/volume-I/cap-09/09-targetrevision.yaml` — exemplo de targetRevision.
- `examples/volume-I/cap-09/09-syncpolicy-auto.yaml` — exemplo de auto-sync.

## Capitulo 10
- `examples/volume-I/cap-10/por-ambiente/project-dev.yaml` — Project dev.
- `examples/volume-I/cap-10/por-ambiente/project-hml.yaml` — Project hml.
- `examples/volume-I/cap-10/por-ambiente/project-prd.yaml` — Project prd.
- `examples/volume-I/cap-10/por-time/project-time-a.yaml` — Project time A.
- `examples/volume-I/cap-10/por-time/project-time-b.yaml` — Project time B.
- `examples/volume-I/cap-10/por-dominio/project-vendas-dev.yaml` — Project vendas dev.
- `examples/volume-I/cap-10/por-dominio/project-vendas-prd.yaml` — Project vendas prd.
- `examples/volume-I/cap-10/segregacao-conceitual.md` — exemplo conceitual de segregacao.

## Capitulo 11
- `examples/volume-I/cap-11/11-applicationset-list.yaml` — exemplo de ApplicationSet (List Generator).

## Capitulo 12
- `examples/volume-I/cap-12/12-appproject-sync-window.yaml` — exemplo de Sync Window em AppProject.

## Capitulo 13
- `examples/volume-I/cap-13/13-ignore-differences-application.yaml` — exemplo basico de Ignore Differences na Application.
- `examples/volume-I/cap-13/13-ignore-differences-jsonpointer.yaml` — exemplo de JSON Pointer.
- `examples/volume-I/cap-13/13-ignore-differences-jq.yaml` — exemplo de jq path expressions.
- `examples/volume-I/cap-13/13-ignore-differences-project.yaml` — exemplo de Ignore Differences em Project.

## Outros exemplos (texto)

### Tipos de revision
Branch (exemplos comuns):
- main
- develop
- feature/nova-funcionalidade

Tag (exemplos):
- v1.0.0
- v1.2.3

Commit (SHA):
- a1b2c3d4e5f6

### Nomenclatura por dominio e ambiente
- vendas-dev
- vendas-hml
- vendas-prd

### Organizacao de Projects (exemplos)
Por ambiente:
- project-dev
- project-hml
- project-prd

Por time:
- project-time-a
- project-time-b

Por dominio:
- project-vendas-dev
- project-vendas-prd

### Exemplo conceitual de segregacao
- Cluster: dev
- Project: project-vendas
- Namespace: vendas-dev
- Application: app-carrinho

### Exemplo conceitual de estrutura (Git Generator)
```
apps/
  ├── app-a/
  │   ├── dev/
  │   └── prd/
  └── app-b/
      ├── dev/
      └── prd/
```

### Exemplo de estrategia por ambiente
```
Ambiente       Sync Policy   Sync Window
Desenvolvimento Auto-Sync    Sem restricao
Homologacao     Auto-Sync    Allow Window
Producao        Manual       Deny Window
```
