# Instalação e fechamento recorrente

## Ativar o agente

1. Crie uma conversa dedicada ou um espaço privado em Claude, ChatGPT ou Gemini. Use o [prompt completo](../prompts/agente-completo.md) como instrução, ou use [AGENTE.md](../AGENTE.md) e forneça as [skills](../skills) quando o ambiente puder ler arquivos. Em uma conversa comum, cole o prompt completo e peça que ele seja usado ao longo daquela conversa. Ao trocar de assistente, leve o último registro do Notion ou um resumo dos campos privados necessários.
2. Configure o [modelo de dados](modelo-de-dados.md) e informe as listas, calendários, janela de trabalho, fuso e margens. Conecte somente os apps necessários que estiverem disponíveis na conta. Quando uma conexão fornecer apenas leitura, o agente entrega as mudanças prontas para você aplicar.
3. Faça um teste de leitura com uma tarefa descartável concluída no dia, uma pendência, um evento fixo e uma página autorizada do Notion. Confirme se o assistente encontrou o status, a data de conclusão e a fonte. Faça esse teste no mesmo tipo de sessão que vai rodar à noite. Para autorizar escrita automática limitada, faça um teste separado em registros fictícios e confira o resultado nos apps.
4. No começo do dia, execute `PLANEJAR HOJE` e registre a linha de base. Durante o dia, conclua tarefas no Google Tasks. Para o que ficar parcial, informe o esforço restante e o bloqueio. No fim, execute `FECHAR` ou use o agendamento abaixo.

## Escolher como disparar a revisão

| Ambiente | Como usar |
| --- | --- |
| Gemini | Conecte Google Workspace. Se o recurso estiver disponível na conta, crie uma ação ou tarefa agendada com o [prompt recorrente](../prompts/fechamento-recorrente.md). Teste se a ação agendada enxerga as tarefas concluídas e os calendários escolhidos. Se ela preparar a resposta antes do horário, confira o corte e refaça `FECHAR` para capturar conclusões posteriores. Forneça os dados do Notion na sessão quando faltar acesso. |
| ChatGPT | Use conversa ou projeto para a operação normal. Se as tarefas agendadas estiverem disponíveis, cole nelas o [prompt recorrente](../prompts/fechamento-recorrente.md) integral. Valide quais apps a própria tarefa pode consultar. Caso só consiga criar um lembrete ou acessar a Agenda, use o lembrete para abrir a sessão e confira o Google Tasks manualmente. |
| Claude | Use conversa ou projeto com as instruções. Autorize os conectores que estiverem disponíveis e teste leitura e escrita separadamente. Se houver agendamento nativo com acesso suficiente às fontes, use o prompt recorrente. Se faltar alguma capacidade, use o fluxo manual abaixo. |

### Quando o conector ou agendamento estiver indisponível

No Google Agenda, crie um evento privado e recorrente **Fechamento de autogestão**, no horário em que você normalmente termina o dia. 21h30 no seu fuso é um ponto de partida ajustável. Inclua um lembrete e o comando `FECHAR`. Ao abrir o assistente, consulte a seção Concluídas do Google Tasks e cole só os dados faltantes no [formato de entrada](modelo-de-dados.md#pacote-para-uso-manual). Copie a saída de volta para o histórico e aplique as mudanças que escolher.

### Confirmar que o agendamento funciona

- Faça uma execução assistida e uma execução agendada de teste. Confira se uma tarefa concluída aparece com data e hora ou confirmação da ocorrência correta, e se a Agenda de amanhã é a mesma observada no app.
- Compare a hora real de coleta com a hora combinada de fechamento. Se a coleta for antecipada, trate como prévia e rode `FECHAR` depois das últimas ações.
- Se o assistente não tiver as metas ou a linha de base, ele entrega diagnóstico parcial. Dê acesso ao registro autorizado do Notion ou forneça um recorte na sessão. Mantenha um único agendamento ativo para o fluxo.
- A integração depende dos recursos e das permissões da sua conta. O repositório fornece as instruções e o fluxo operacional. O agendamento é criado e testado na conta em que vai rodar.

## Referências dos aplicativos

- [Ações agendadas no Gemini](https://support.google.com/gemini/answer/16316416) e [Google Tasks no Gemini](https://support.google.com/gemini/answer/15230285).
- [Tarefas agendadas no ChatGPT](https://help.openai.com/en/articles/10291617-tasks-in-chatgpt) e [Notion no ChatGPT](https://help.openai.com/en/articles/12532955-notion-app-with-sync).
- [Conectores no Claude](https://support.anthropic.com/en/articles/11817150-connect-your-tools-to-unlock-a-smarter-more-capable-ai-companion).
- [Listagem de tarefas e filtro de concluídas da API do Google Tasks](https://developers.google.com/workspace/tasks/reference/rest/v1/tasks/list).
