<!--
  RASCUNHO do README do perfil da organização MecaniSys.
  ONDE PUBLICAR: crie/abra o repositório especial `MecaniSys/.github`
  (nome exatamente `.github`) e cole este conteúdo no `profile/README.md`
  dele — é o que o GitHub exibe em https://github.com/MecaniSys .
  Este arquivo local é só o rascunho versionado; a publicação é manual.
-->

# MecaniSys 🔧

SaaS para gestão de oficinas mecânicas: clientes, catálogo de serviços e
pacotes, ordens de serviço e assinaturas — cada oficina como um tenant isolado.

## Repositórios

| Repositório | O quê |
|---|---|
| [`backend-app`](https://github.com/MecaniSys/backend-app) | API REST (Java 21 · Spring Boot · PostgreSQL + Flyway · JWT RS256). É aqui que o produto evolui. |
| `infra-*` | GitOps/Kustomize dos ambientes (`overlays/dev`, `overlays/prod`) — atualizado automaticamente pelo CI do backend (ver `infra-repo.yml`). |
| Frontend | Em planejamento — consumirá a API segundo [`docs/api-frontend.md`](https://github.com/MecaniSys/backend-app/blob/develop/docs/api-frontend.md). |

## Como funciona

- `develop` → builda a imagem e atualiza o ambiente **DEV**; `main` → promove para **PROD**.
- Desenvolvedores começam pelo `README.md` do `backend-app` (quickstart com Docker Compose).
- Documentos de referência: [guia da API para o frontend](https://github.com/MecaniSys/backend-app/blob/develop/docs/api-frontend.md) ·
  [modelo de dados](https://github.com/MecaniSys/backend-app/blob/develop/docs/relacionamentos-banco.md).

## Stack

Java 21 · Spring Boot · PostgreSQL 17 · Flyway · Docker · Kubernetes (Kustomize) · GitHub Actions.
