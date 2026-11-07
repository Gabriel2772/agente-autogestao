# Prompt independente para fechamento recorrente

Preencha os campos entre colchetes com seus dados antes de enviar ao agendador. Use o mesmo fuso no Google Agenda, na configuração do assistente e no relatório.

```text
Agende este fechamento diariamente às [21:30], fuso [America/Sao_Paulo].
Use somente Google Tasks, Google Agenda e Notion, conforme as ferramentas autorizadas nesta rotina.
Listas do Tasks: [Ações, Metas semanais, Metas mensais].
Calendários: [nomes].
Janelas pessoais de amanhã: [horários].
Margem: [20% de cada janela livre].
Notion: [página privada ou referência do plano e do histórico].

Em cada execução, produza uma revisão em português. Informe data local, hora real de coleta e cobertura de cada fonte. Recupere o plano original do dia no Notion quando disponível. No Tasks, confira ocorrências planejadas e conclusões desde a meia-noite local até o corte. Use o horário real de conclusão, inclusive para tarefas originalmente datadas de outro dia. Se a ferramenta expuser filtros da API, peça também as concluídas ocultas e percorra a paginação. Nunca deduza conclusão ou falta de execução pela ausência numa lista incompleta. Separe concluídas, parciais, não iniciadas confirmadas, desconhecidas e conclusões fora do plano. Sem linha de base, não calcule taxa.

Confira a Agenda de amanhã, unindo intervalos ocupados que se sobrepõem. Desconte transições conhecidas e a margem de cada janela. Reestime o esforço restante, respeite dependências e encaixe apenas trabalho que couber na janela adequada. Para duração parcial desconhecida, peça uma estimativa ou deixe a proposta condicional. Liste o efeito sobre metas semanais, mensais e marcos. Separe a previsão revisada do prazo acordado e sinalize o que exige decisão.

Entregue três blocos: Execução e cobertura; Amanhã e capacidade; Impacto e decisões. Use a chave FECHO:<data local>. Se a coleta foi antecipada, chame a revisão de parcial. Se faltar acesso a concluídas, peça a seção Concluídas ou confirmação das ocorrências relevantes. Apresente propostas sem alterar os apps. Ao concluir, entregue um bloco pronto para o usuário registrar no Notion. Use no máximo uma pergunta agrupada.
```
