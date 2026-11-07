# Exemplo fictício: Eisenhower e horário de energia

**Preferências declaradas.** Fuso America/Sao_Paulo. Trabalho 09h–12h e 13h–17h; janela noturna opcional 19h–21h. Energia alta na manhã, média na tarde e baixa à noite. Compromissos **fixos** no Google Agenda: reunião 10h30–11h e consulta 14h–15h. Margem de 20% de **cada janela livre**, conforme a skill Capacidade real.

| ID | Ação | Impacto e prazo real | Energia | Quadrante |
| --- | --- | --- | --- | --- |
| A-101 | Desenvolver protótipo para o marco M-01 (60 min) | Alto impacto; sem prazo imediato | Alta | Q2 |
| A-102 | Revisar entrega contratual (45 min) | Alto impacto; vence hoje às 13h | Alta | Q1 |
| A-103 | Responder solicitação administrativa (20 min) | Urgente até 17h, mas pouco impacto no objetivo | Baixa | Q3 |
| A-104 | Organizar notas antigas (15 min) | Sem impacto ou prazo relevante; opcional | Baixa | Q4 |

## Resultado esperado do planejamento

| Horário | Item | Decisão |
| --- | --- | --- |
| 09h–10h | A-101 (Q2) | Protege o primeiro bloco de foco da manhã |
| 10h30–11h | Reunião fixa | Intocável |
| 11h–11h45 | A-102 (Q1) | Conclui antes do prazo de 13h |
| 14h–15h | Consulta fixa | Intocável |
| 15h30–15h50 | A-103 (Q3) | Tarefa operacional após o foco e antes do prazo |
| 19h–19h15 | A-104 (Q4), se o usuário quiser mantê-la | Opcional, leve e somente por haver janela noturna permitida |

**Checagem de capacidade.** As janelas livres brutas são 09h–10h30 (90 min), 11h–12h (60 min), 13h–14h (60 min), 15h–17h (120 min) e 19h–21h (120 min). Descontando 20% de cada uma (18 + 12 + 12 + 24 + 24 min), há 360 min úteis no total. As quatro ações somam 140 min e cabem sem usar a margem. As lacunas entre blocos podem absorver transições e interrupções dentro da capacidade reservada; se houver transições conhecidas adicionais, recalcule.

**Replanejamento.** Se A-102 passar a vencer às 10h, sua execução deve preceder A-101, e o foco Q2 vai para a próxima janela adequada. Se a janela noturna não estiver autorizada, A-104 fica fora da agenda, não é transferida para depois das 21h. O agente registra a alteração e não muda compromissos fixos.
