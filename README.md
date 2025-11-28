# DailyQuest Docs

Documentação do projeto com MkDocs Material.

## Quick Start

```bash
# Instalar dependências
pip install mkdocs mkdocs-material

# Rodar localmente
mkdocs serve

# Acessar: http://localhost:8000
```

## Estrutura

```
docs/
├── index.md       # Página inicial
├── backlog.md     # Product backlog
├── banco.md       # Modelagem DB
├── diagrama.md    # Diagramas UML
├── prototipo.md   # Protótipos UI
└── assets/        # Imagens
```

## Build

```bash
mkdocs build   # Gera site estático em /site
```