---
name: capacidade-real
description: "Use para planejar hoje ou amanhã, decidir a próxima ação ou verificar se uma entrega cabe na agenda."
---

# Capacidade real

1. Determine as janelas que a pessoa realmente disponibilizou e os compromissos dos calendários selecionados. Use o mesmo fuso e recorte os eventos às janelas. Faça a união das janelas de disponibilidade. Faça também a união dos intervalos ocupados, incluindo transições conhecidas, para contar uma sobreposição uma vez. Classifique eventos de dia inteiro conforme a disponibilidade observada ou confirmada.
2. Subtraia a união ocupada da disponibilidade para obter janelas livres. Desconte a reserva em cada janela livre. Por padrão use 20% arredondados para cima em minutos, uma convenção ajustável do agente. Trate blocos flexíveis já reservados como ocupados ou desalocados explicitamente no cenário que os move.
3. Filtre ações pelo contexto, pré-requisitos, duração, divisibilidade e energia. Use a faixa alta de uma estimativa incerta para um compromisso firme. Para trabalho indivisível, exija uma janela contígua. Para trabalho divisível, aloque partes com resultado intermediário e conte transições. Se agenda ou energia estiverem incompletas, mostre o que é hipótese.
4. Entre ações elegíveis, proteja compromissos em risco e passos que liberam entregas. Dimensione novos inícios pelo gargalo real, como um único bloco de foco ou aprovação. Entre ações de impacto semelhante, priorize concluir a entrega em curso. Reserve a proteção e mostre o que ficou fora.

**Saída** | janelas brutas e úteis, carga por janela, folga, tarefas adiadas e justificativa.

**Origem** | GTD, critérios de engajamento. A Meta, gargalo, trabalho em curso e fluxo. O Ano de 12 Semanas, blocos de execução.
