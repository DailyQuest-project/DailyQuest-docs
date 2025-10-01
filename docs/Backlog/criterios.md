# CRITÉRIOS DE ACEITE - Daily Quest

## **Visão do Produto**
Daily Quest é uma plataforma web de gerenciamento de hábitos gamificada que ajuda usuários a criar, acompanhar e manter hábitos saudáveis através de mecânicas de jogos (XP, níveis, conquistas, streaks).

---

## **US#1 - Cadastro de Usuário**
**Como** usuário novo  
**Quero** me cadastrar na plataforma  
**Para** começar a usar o sistema de hábitos

**Critérios de Aceite:**

- [ ] Formulário deve conter campos obrigatórios: email, senha, nome de usuário
- [ ] Email deve ser único no sistema (validação de duplicata)
- [ ] Senha deve ter mínimo 8 caracteres com validação
- [ ] Validação de formato de email válido
- [ ] Confirmação de senha deve coincidir com senha original
- [ ] Mensagem de sucesso/erro clara para o usuário
- [ ] Redirecionamento automático para página de login após cadastro bem-sucedido

---

## **US#2 - Login de Usuário**
**Como** usuário cadastrado  
**Quero** fazer login  
**Para** acessar minha conta pessoal

**Critérios de Aceite:**

- [ ] Login deve funcionar com email e senha
- [ ] Validação de credenciais no backend
- [ ] Geração e armazenamento de token JWT para sessão
- [ ] Opção "Lembrar-me" para sessão persistente (opcional)
- [ ] Mensagem de erro clara em caso de credenciais inválidas
- [ ] Redirecionamento para dashboard principal após login bem-sucedido

---

## **US#3 - Criar Hábito**
**Como** usuário logado  
**Quero** criar um novo hábito  
**Para** começar a acompanhar minhas atividades

**Critérios de Aceite:**

- [ ] Formulário com campos: título (obrigatório), descrição (opcional), dificuldade
- [ ] Seleção de tipo: Hábito Recorrente ou Tarefa Única
- [ ] Definir frequência (diária, semanal, flexível)
- [ ] Opção de adicionar tags existentes ou criar novas (opcional)
- [ ] Preview da recompensa em XP baseada na dificuldade selecionada
- [ ] Validação de campos obrigatórios com feedback visual
- [ ] Feedback visual de sucesso após criação do hábito

---

## **US#4 - Marcar Hábito como Concluído**
**Como** usuário logado  
**Quero** marcar um hábito como concluído  
**Para** registrar meu progresso

**Critérios de Aceite:**

- [ ] Botão/checkbox visível para marcar conclusão
- [ ] Registro automático da data e hora de conclusão
- [ ] Cálculo e atribuição automática de XP
- [ ] Feedback visual imediato (animação, notificação +XP)
- [ ] Atualização de streak se aplicável ao tipo de hábito
- [ ] Prevenção de conclusão duplicada no mesmo dia (para hábitos diários)
- [ ] Persistência da conclusão no banco de dados

---

## **US#5 - Visualizar XP e Nível**
**Como** usuário logado  
**Quero** visualizar meu nível e experiência atual  
**Para** acompanhar minha evolução

**Critérios de Aceite:**

- [ ] Barra de progresso de XP sempre visível na interface
- [ ] Nível atual exibido claramente ao lado do nome do usuário
- [ ] Informação "XP atual / XP necessário para próximo nível"
- [ ] Animação visual ao subir de nível
- [ ] Histórico de níveis alcançados acessível no perfil
- [ ] Cálculo correto de XP necessário por nível (progressão matemática)
- [ ] Atualização em tempo real após ganhar XP

---

## **US#6 - Listar Hábitos Ativos**
**Como** usuário logado  
**Quero** ver minha lista de hábitos ativos  
**Para** gerenciar minhas atividades

**Critérios de Aceite:**

- [ ] Lista ordenada por data de criação ou prioridade configurável
- [ ] Separação visual clara entre Hábitos Recorrentes e Tarefas Únicas
- [ ] Indicador visual de status (concluído hoje/não concluído)
- [ ] Exibir streak atual para hábitos que possuem sequência
- [ ] Exibir deadline para tarefas únicas
- [ ] Opção de alternar visualização para hábitos inativos/arquivados
- [ ] Performance adequada com paginação se necessário

---

## **US#7 - Criar e Gerenciar Tags**
**Como** usuário logado  
**Quero** criar e gerenciar tags  
**Para** categorizar meus hábitos

**Critérios de Aceite:**

- [ ] Modal/interface para criar nova tag com nome e cor
- [ ] Funcionalidade de editar tags existentes
- [ ] Opção de excluir tags com confirmação de segurança
- [ ] Sugestões de tags pré-definidas (saúde, trabalho, estudo, etc.)
- [ ] Validação para evitar nomes de tags duplicados
- [ ] Limite de caracteres no nome da tag (máximo 20)
- [ ] Preview visual da tag antes de salvar

---

## **US#8 - Criar Tarefas com Deadline**
**Como** usuário logado  
**Quero** criar tarefas únicas com deadline  
**Para** gerenciar atividades pontuais

**Critérios de Aceite:**

- [ ] Formulário com campos: título, descrição, deadline (obrigatório)
- [ ] Seletor de data e hora para deadline
- [ ] Definir nível de dificuldade (impacta cálculo de XP)
- [ ] Indicador visual de urgência baseado em dias restantes
- [ ] Notificação automática quando prazo está próximo (opcional)
- [ ] Funcionalidade de marcar como concluída
- [ ] Recompensa de XP ao concluir tarefa

---

## **US#9 - Visualizar Histórico de Progresso**
**Como** usuário logado  
**Quero** visualizar meu histórico de progresso  
**Para** acompanhar minha evolução

**Critérios de Aceite:**

- [ ] Calendário visual mostrando dias com atividades concluídas
- [ ] Lista cronológica de todas as conclusões de hábitos/tarefas
- [ ] Filtro por período (última semana, último mês, último ano)
- [ ] Filtro por hábito específico
- [ ] Estatísticas básicas: total de conclusões, taxa de sucesso
- [ ] Opção de exportação de dados para análise externa (opcional)
- [ ] Gráficos simples de progresso ao longo do tempo

---

## **US#10 - Editar ou Excluir Hábitos**
**Como** usuário logado  
**Quero** editar ou excluir hábitos existentes  
**Para** manter minha lista atualizada

**Critérios de Aceite:**

- [ ] Botão de "Editar" visível em cada hábito na lista
- [ ] Modal/página de edição com todos os campos preenchidos
- [ ] Validação de campos ao salvar edição
- [ ] Confirmação obrigatória antes de excluir hábito
- [ ] Manutenção do histórico de conclusões ao editar
- [ ] Opção de arquivar hábito ao invés de excluir permanentemente
- [ ] Feedback visual claro de sucesso/erro após operação

---

## **US#11 - Definir Dificuldades para Hábitos**
**Como** usuário logado  
**Quero** definir dificuldades para meus hábitos  
**Para** ganhar experiência proporcional ao esforço

**Critérios de Aceite:**

- [ ] Três níveis de dificuldade disponíveis: Fácil, Médio, Difícil
- [ ] XP base diferenciado por dificuldade: Fácil (15 XP), Médio (25 XP), Difícil (40 XP)
- [ ] Indicador visual claro da dificuldade na lista de hábitos
- [ ] Possibilidade de alterar dificuldade de hábitos existentes
- [ ] Preview da quantidade de XP ao criar/editar hábito
- [ ] Cálculo correto implementado no sistema de XP
- [ ] Exibição da dificuldade em todos os locais onde o hábito aparece

---

## **US#12 - Filtrar Hábitos por Tag**
**Como** usuário logado  
**Quero** filtrar hábitos por tag  
**Para** organizar melhor minha visualização

**Critérios de Aceite:**

- [ ] Dropdown/chips de seleção com todas as tags disponíveis
- [ ] Capacidade de filtrar por múltiplas tags simultaneamente
- [ ] Atualização imediata da lista ao aplicar filtros
- [ ] Indicador visual claro de quais filtros estão ativos
- [ ] Botão para limpar todos os filtros aplicados
- [ ] Contador mostrando quantidade de hábitos filtrados
- [ ] Performance adequada mesmo com muitas tags

---

## **US#13 - Ver Estatísticas de Frequência**
**Como** usuário logado  
**Quero** ver estatísticas detalhadas de frequência  
**Para** entender meus padrões de comportamento

**Critérios de Aceite:**

- [ ] Gráfico de frequência de conclusão por dia da semana
- [ ] Análise de horários mais produtivos do usuário
- [ ] Ranking de hábitos mais/menos cumpridos
- [ ] Taxa de sucesso por categoria/tag de hábitos
- [ ] Gráficos visuais diversos (barras, pizza, linhas)
- [ ] Comparação de desempenho entre períodos diferentes
- [ ] Sistema de insights automáticos baseado nos dados (opcional)

---

## **US#14 - Definir Metas de Sequência (Streaks)**
**Como** usuário logado  
**Quero** acompanhar sequências consecutivas de conclusões  
**Para** me motivar a manter consistência

**Critérios de Aceite:**

- [ ] Contador automático de dias consecutivos (streak atual)
- [ ] Indicador visual de streak ativo (ícone 🔥 ou similar)
- [ ] Configuração de meta de streak por hábito
- [ ] Alerta/notificação quando streak está em risco de quebrar
- [ ] Histórico de maior streak já alcançada por hábito
- [ ] Sistema de bônus de XP por milestones de streak (7, 30, 100 dias)
- [ ] Reset automático de streak quando hábito não é concluído

---

## **US#15 - Receber Notificações de Hábitos Pendentes**
**Como** usuário logado  
**Quero** receber lembretes de hábitos não concluídos  
**Para** não esquecer de minhas atividades

**Critérios de Aceite:**

- [ ] Configuração de horário de lembrete individual por hábito
- [ ] Notificações in-app visíveis na interface
- [ ] Opção de notificações por email (opcional)
- [ ] Sistema de push notifications se aplicável (opcional)
- [ ] Configuração global para ligar/desligar todas as notificações
- [ ] Funcionalidade de snooze para adiar lembretes
- [ ] Personalização de mensagem de lembrete

---

## **US#16 - Exportar Dados**
**Como** usuário logado  
**Quero** exportar meus dados pessoais  
**Para** backup ou análise em ferramentas externas

**Critérios de Aceite:**

- [ ] Formatos de exportação disponíveis: JSON e CSV
- [ ] Inclusão de dados: hábitos, conclusões, estatísticas, tags
- [ ] Botão de exportação facilmente acessível no perfil
- [ ] Download automático do arquivo após processamento
- [ ] Confirmação visual de que exportação foi bem-sucedida
- [ ] Limite de frequência para prevenir abuso (máximo 1x por dia)
- [ ] Arquivo gerado deve estar formatado corretamente

---

## **US#17 - Personalizar Perfil**
**Como** usuário logado  
**Quero** personalizar informações do meu perfil  
**Para** tornar a experiência mais pessoal

**Critérios de Aceite:**

- [ ] Alteração de nome de usuário com validação de unicidade
- [ ] Upload de avatar/foto de perfil com redimensionamento automático
- [ ] Alteração de email com processo de verificação
- [ ] Alteração de senha exigindo senha atual para confirmação
- [ ] Campo de bio/descrição pessoal (máximo 200 caracteres)
- [ ] Configuração de preferências de idioma da interface
- [ ] Configuração de timezone para horários corretos
- [ ] Validação completa de todos os campos modificados

---

## **US#18 - Visualizar Conquistas/Badges**
**Como** usuário logado  
**Quero** ver conquistas desbloqueadas baseadas no meu progresso  
**Para** me sentir recompensado pelo esforço

**Critérios de Aceite:**

- [ ] Galeria com todas as conquistas disponíveis no sistema
- [ ] Indicação visual clara entre badges desbloqueadas e bloqueadas
- [ ] Conquistas variadas: primeira conclusão, streak 7 dias, nível 10, etc.
- [ ] Animação especial ao desbloquear nova conquista
- [ ] Notificação push/popup quando conquista é obtida
- [ ] XP bônus automático ao desbloquear conquista importante
- [ ] Barra de progresso mostrando progresso para próximas conquistas

---

## **US#19 - Ver Dashboard com Resumo**
**Como** usuário logado  
**Quero** visualizar dashboard com métricas consolidadas  
**Para** análise rápida do meu progresso temporal

**Critérios de Aceite:**

- [ ] Cards com métricas principais: taxa de sucesso, streak atual, XP total
- [ ] Gráfico de conclusões de hábitos ao longo do tempo
- [ ] Comparação automática com períodos anteriores (% de melhora/piora)
- [ ] Lista dos hábitos mais cumpridos no período selecionado
- [ ] Indicador de metas vs realizado no período
- [ ] Filtros por período: semana atual, mês atual, personalizado
- [ ] Design responsivo que funciona em dispositivos móveis

---

## **US#20 - Ganhar Moedas Virtuais**
**Como** usuário logado  
**Quero** acumular moedas virtuais ao completar atividades  
**Para** ter sistema de recompensas adicional

**Critérios de Aceite:**

- [ ] Moedas ganhas automaticamente junto com XP
- [ ] Quantidade de moedas proporcional à dificuldade do hábito
- [ ] Contador de moedas sempre visível na interface principal
- [ ] Histórico detalhado de ganhos e gastos de moedas
- [ ] Base para futura loja de recompensas virtuais (opcional para MVP)
- [ ] Persistência correta das moedas no banco de dados
- [ ] Sistema balanceado para evitar inflação de moedas

---

## **US#21 - Modo Escuro (Dark Mode)**
**Como** usuário logado  
**Quero** alternar entre modo claro e escuro  
**Para** personalizar minha experiência visual

**Critérios de Aceite:**

- [ ] Toggle/switch facilmente acessível para alternar modos
- [ ] Persistência da preferência entre sessões do usuário
- [ ] Todos os componentes da interface adaptados ao modo escuro
- [ ] Contraste adequado para garantir acessibilidade
- [ ] Transição suave e visualmente agradável entre modos
- [ ] Ícone indicativo claro do modo atualmente ativo
- [ ] Opcional: sincronização com preferência do sistema operacional

---

*Documento atualizado em: 30 de setembro de 2025*