# Modelo de dados

## Notion

Crie uma página privada chamada **Autogestão**, com estas bases. Os nomes de propriedades podem variar, desde que o agente conheça o mapeamento.

| Base | Campos mínimos |
| --- | --- |
| Objetivos | ID, resultado esperado, indicador, unidade, linha de base, alvo, data-alvo, estado |
| Projetos | ID, relação com objetivo, entrega e aceite, prioridade, prazo acordado, previsão atual, estado |
| Marcos | ID, relação com projeto, entrega e aceite, dependências, prazo acordado, previsão, IDs das metas no Tasks |
| Histórico | Chave e versão, fuso, horário de corte, plano de referência por ocorrência, cobertura e fonte, fatos da execução, proposta, decisão e efeitos por aplicativo |

Adicione esforço restante, datas de disponibilidade e responsáveis onde forem úteis para dependências. Use um registro de histórico por data local. Antes da execução, salve as ocorrências planejadas e os minutos estimados nessa data. Anexe fatos posteriores e mantenha o plano original mesmo quando alterar a agenda.

## Google Tasks

Crie três listas, **Metas mensais**, **Metas semanais** e **Ações**. Use título curto e notas como estas. Registre o ID nativo quando a integração o expuser.

```text
ID: A-001
Pai: S-003
Projeto: P-002
Marco: M-004
Concluído quando: proposta revisada e aprovada na versão atual
Esforço restante: 45 min
Energia: alta
Impacto: libera o marco M-004
Prazo firme: nenhum (ou AAAA-MM-DD HH:MM com fuso)
Depende de: A-000
Divisível: não
```

Nas metas, registre o critério mensurável e o período. Use a data da tarefa como data-alvo, e a Agenda para hora e duração. Mantenha a ocorrência de cada recorrência separada na linha de base. Evite marcar uma meta como concluída apenas porque todas as ações foram feitas. Confira o resultado.

## Google Agenda

Escolha os calendários que bloqueiam disponibilidade, incluindo os compromissos pessoais relevantes. Crie um calendário privado **Blocos de execução** se quiser separar reservas flexíveis. Use `[A-001] Revisar proposta` e anote ID da tarefa, flexibilidade e chave da ocorrência. Na capacidade, um bloco existente só volta a ser oferta se o usuário tiver delegado sua movimentação e ele entrar explicitamente na proposta. Some o trabalho alocado nele uma única vez.

## Preferências de trabalho e energia

Informe a janela normal de trabalho, as janelas noturnas **opcionais** e os horários em que percebe maior ou menor energia (por exemplo: foco alto de manhã, tarefas administrativas à tarde, atividades leves à noite). Essa preferência não é uma disponibilidade presumida: um horário fora da janela autorizada continua indisponível. O agente calcula a urgência a partir dos prazos reais e consequências, e a importância a partir de objetivos, marcos e impacto; evite manter quadrantes estáticos nas tarefas. Compromissos com hora no Google Agenda permanecem fixos salvo autorização específica.

## Pacote para uso manual

```text
FECHAR AAAA-MM-DD | fuso America/Sao_Paulo | corte 21:30
Plano inicial: A-001 45 min; A-002 30 min
Tasks: A-001 concluída às 18h; A-002 parcial, faltam 15 min
Cobertura: lista Ações e seção Concluídas conferidas até o corte
Amanhã: janela 09–12; reunião 10–11; transição 10 min; energia média
Projetos: M-004 vence dia 18; critério e dependências ...
Mudança de prioridade ou bloqueio: ...
```

Se houver uma leitura incompleta, marque a limitação e confirme manualmente só os registros relevantes. Use referências fictícias para testes e mantenha dados reais no ambiente privado.
