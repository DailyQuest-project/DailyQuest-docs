# Daily Quest

Plataforma de hábitos gamificada que transforma sua rotina em uma aventura RPG.

## Contexto

Evolução de um projeto da disciplina de Orientação a Objetos, inspirado no Habitica. A versão atual implementa:

- Arquitetura de microserviços com FastAPI
- Sistema de gamificação expandido
- Interface moderna com Next.js
- Analytics e progressão personalizados
- Sistema flexível de frequência de hábitos

## Arquitetura

| Serviço | Tecnologia | Porta |
|---------|------------|-------|
| **Frontend** | Next.js 14, React 19, TypeScript, TailwindCSS | 3000 |
| **API** | FastAPI, SQLAlchemy, Alembic | 8000 |
| **Auth** | FastAPI, JWT | 8001 |
| **Database** | PostgreSQL 15 | 5432 |

## Usuários de Teste

| Usuário | Email | Senha | Descrição |
|---------|-------|-------|-----------|
| `testuser` | test@example.com | `testpass123` | Usuário básico para testes |
| `demo` | demo@dailyquest.com | `demo123` | Usuário avançado (Nível 8, histórico de 15 dias) |

## Quick Start

```bash
# Subir todos os serviços
docker compose up --build

# Acessar
# Frontend: http://localhost:3000
# API Docs: http://localhost:8000/docs
# Auth: http://localhost:8001/docs
```

## Funcionalidades

### Sistema de Hábitos
- Hábitos recorrentes com frequências configuráveis (diário, semanal, etc.)
- Tarefas únicas (To-Dos) com deadline
- Sistema de tags para organização
- Filtros avançados

### Gamificação
- Sistema de XP e níveis
- Dificuldades que impactam recompensas
- Conquistas desbloqueáveis
- Sistema de streaks (sequências)
- Moedas virtuais

### Dashboard e Analytics
- Métricas de progresso
- Histórico completo de conclusões
- Estatísticas de frequência e padrões
- Visualizações gráficas

### Personalização
- Perfil customizável
- Dark mode
- Preferências de notificações

## Cronograma

| Marco | Data |
|-------|------|
| Início do projeto | 28/09/2024 |
| Entrega MVP | 30/11/2024 |

**Metodologia:** Sprints semanais

## Repositórios

- `DailyQuest-web` - Frontend Next.js
- `DailyQuest-api` - Backend principal
- `DailyQuest-auth` - Serviço de autenticação
- `DailyQuest-docs` - Documentação MkDocs

## Status

✅ MVP Concluído - Novembro/2024

**Última Atualização:** 28/11/2024