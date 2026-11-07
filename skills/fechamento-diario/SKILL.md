---
name: fechamento-diario
description: "Use no fim do dia ou para corrigir um fechamento anterior com evidência nova."
---

# Fechamento diário

1. Defina data local e corte observado. Recupere a linha de base original e os IDs de ocorrência. Busque conclusões entre a meia-noite local e o menor valor entre o corte e a próxima meia-noite local, e recupere estados atuais das ocorrências planejadas. Busque conclusões pela data em que ocorreram, inclusive de tarefas originalmente vencidas em outro dia. Se a ferramenta expuser parâmetros da API Tasks, use `showCompleted=true`, `showHidden=true` e pagine todas as listas incluídas. Converta timestamps para o fuso local antes de filtrar e excluir o limite final da próxima data. Se a ferramenta mostrar só tarefas abertas, informe a cobertura parcial e solicite a seção Concluídas ou confirmação manual.
2. Aplique a classificação por ocorrência. **Concluída** quando o critério tem evidência na data do fechamento. **Parcial** quando há avanço confirmado e resta trabalho. **Não executada** quando o usuário ou evidência direta confirma que não começou. **Desconhecida** quando falta evidência, inclusive tarefa ausente, aberta sem informação de esforço, ou leitura desatualizada. Um item já concluído antes do dia é uma divergência da linha de base. Registre-o à parte como conclusão anterior e preserve o denominador original. Separe conclusões não planejadas, cancelamentos e mudanças autorizadas.
3. Reporte concluídas de N previstas e, se houver U desconhecidas, faixa de concluídas possíveis de C/N a (C+U)/N. Se N = 0, use não aplicável. Se faltar a linha de base, mostre fatos de execução observados e deixe o placar indisponível. Mantenha parciais fora do numerador. Conte cada recorrência apenas uma vez por ocorrência.
4. Passe o que resta confirmado ao replanejamento. Retenha estados desconhecidos para conciliar. Atualize o mesmo fechamento quando houver confirmação posterior. Se a captura ocorrer antes da hora combinada, chame de parcial, informe o corte e peça atualização se houve ação depois dele.

**Origem** | Hábitos Atômicos, rastreio e retomada. O Ano de 12 Semanas, distinção entre táticas executadas e resultado. Checklist, confirmação baseada em evidência. As classes e faixas são convenções do projeto.
