# Evolução do Diagrama UML - Daily Quest

## Visão Geral

Este documento apresenta a evolução do diagrama UML do sistema Daily Quest, desde a primeira versão desenvolvida na disciplina de Orientação a Objetos até a versão otimizada atual.

---

## Primeira Versão - Diagrama UML

![Primeira versão do diagrama UML](../assets/UML%20-%20HABITICA.png)

## Diagrama UML - Versão Atual

<iframe frameborder="0" style="width:100%;height:1124px;" src="https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&dark=0#G1b5OH_JKeCO5h0ZbnUwoV-nQI5skubfuD"></iframe>


# Evolução do Diagrama UML - Sistema Daily Quest

## Visão Geral
Este documento apresenta a evolução do diagrama de classes UML do sistema Daily Quest, desde a versão inicial simplificada até a versão expandida atual.

## Versão Inicial (Simplificada)

A primeira versão apresentava uma estrutura mais enxuta e focada:

### Características Principais:
- **Classes principais**: User, Task (abstrata), Habit, ToDo, Tag, Data
- **Gamificação básica**: Status positivo/negativo simples
- **Estrutura minimalista**: Foco apenas nas funcionalidades essenciais
- **Persistência centralizada**: Classe Data para operações de I/O
- **Tags simples**: Estrutura boolean básica

### Características:
- 6 classes principais
- Hierarquia simples com Task abstrata
- Métodos de filtro básicos
- Sem sistema de notificações ou achievements

## Versão Atual (Expandida)

A versão atual foi expandida significativamente, incorporando um sistema completo de gamificação:

### Características Principais:
- **Classes expandidas**: User, Task, Habit, ToDo, Tag, Notification, Achievement, UserStats, XpCalculator
- **Sistema de gamificação completo**: XP, níveis, moedas, conquistas
- **Estatísticas detalhadas**: UserStats rastreando completions, streaks, atividades
- **Sistema de notificações**: Classe dedicada com tipos variados e agendamento
- **Exportação de dados**: Múltiplos formatos (JSON, CSV, PDF)
- **Tags avançadas**: Com contadores de uso

### Melhorias:
- Expansão de ~100% no número de classes
- Sistema de recompensas e progressão
- Notificações programáveis
- Rastreamento completo de estatísticas
- Sistema de conquistas por categoria

## Principais Mudanças

| Aspecto | Versão Inicial | Versão Atual |
|---------|---------------|--------------|
| Total de Classes | 6 | 12+ |
| Sistema de XP | Inexistente | Completo com calculator |
| Notificações | Não | Classe dedicada |
| Achievements | Não | Sistema completo |
| Exportação | Básica | Multi-formato |
| Estatísticas | Não | UserStats dedicada |

## Conclusão

A evolução do diagrama reflete a expansão do sistema de um aplicativo simples de produtividade para uma plataforma completa de gamificação de hábitos, incorporando elementos motivacionais, rastreamento detalhado e recursos avançados de engajamento do usuário.
*Última atualização: 30 de setembro de 2025*