# Ações reutilizáveis do GitHub Actions — ToggleMaster

Este repositório contém composite actions consumidas pelos workflows dos serviços em `toggle-master-pipeline-workflows`.

## Ações

- `/.github/actions/trivy-fs`: analisa dependências no sistema de arquivos e falha ao encontrar vulnerabilidades CRITICAL.
- `/.github/actions/docker-build-scan`: constrói a imagem do serviço e falha ao encontrar vulnerabilidades CRITICAL.

Os consumidores devem fixar este repositório em uma tag de release revisada ou SHA de commit. Estas actions não publicam imagens, acessam a AWS nem fazem deploy no Kubernetes.
