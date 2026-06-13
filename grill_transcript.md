# Transcript da Sessão Grill-Me — Blueprint AS-IS Balcão Virtual TRT18

**Data:** 2026-06-12/13  
**Metodologia:** Grill-Me (Matt Pocock / Claude Code Skills v2.9.0)  
**Objetivo:** Definir as decisões metodológicas para elaboração do Service Blueprint AS-IS da jornada "Balcão Virtual do TRT18", seguindo Shostack (Physical Evidence, Customer Actions, Frontstage, Backstage, Support Processes + linhas divisórias + fail points).  
**Artefato de contexto:** `B_relatorio_assistente_v3.md`  
**Artefato produzido:** `C_blueprint_asis.md`

---

## Decisões Locked-In (Resumo Executivo)

| # | Decisão | Resposta |
| :--- | :--- | :--- |
| 1 | Persona primária | Cidadão leigo hipossuficiente |
| 2 | Escopo de canais | Três canais em profundidade igual: Web/Celeste→Zoom (A) + WhatsApp Atermação (B) + PID Físico (C) |
| 3 | Tratamento de `[H_*]` | Incluir como fail points com notação `⚠ [H_nome]` + `★FP` |
| 4 | Camada Normativos e Governança | 6ª faixa própria abaixo de Processos de Suporte, separada por linha regulatória |
| 5 | Granularidade de etapas | 4 etapas macro mantidas |
| 6 | Representação dos canais no artefato | Sub-linhas A/B/C nas etapas 1–2; marcador *(convergência)* nas etapas 3–4 |

---

## Transcrição Completa

---

### Q1/6 — Persona primária

**Pergunta formulada:**
> Qual é a persona primária do blueprint? O v3 menciona dois perfis distintos com jornadas materialmente diferentes: o cidadão leigo hipossuficiente (que pode falhar na triagem da Celeste por analfabetismo funcional/digital) e o advogado (que navega o sistema com fluência e usa o Balcão como canal de conveniência). Essas jornadas têm fail points, evidências físicas e ações de frontstage muito diferentes.

**Resposta recomendada pelo Claude:**
Persona primária = cidadão leigo hipossuficiente. Rationale: é onde estão concentrados os fail points críticos do v3 (`[H_Interface_Celeste]`, `[H_Fila]`, `[H_Autenticacao]`, `[H_Deslocamento_Contraditório]`) e onde o impacto de exclusão é mais severo. O advogado pode ser tratado como persona secundária com nota, sem desdobrar uma lane paralela completa.

**Resposta do usuário:**
> "o cidadão é a persona primária"

**Decisão locked-in:** Persona primária = cidadão leigo hipossuficiente. O advogado permanece como persona secundária implícita, sem lane dedicada no blueprint.

---

### Q2/6 — Escopo de canais

**Pergunta formulada:**
> O blueprint cobre os três canais de entrada (Celeste→Zoom, WhatsApp atermação, PID físico) ou apenas o canal principal Celeste→Zoom? O v3 documenta três pontos de entrada distintos para o cidadão leigo: (1) o portal web com triagem pela Celeste, (2) o WhatsApp 62 3222-5570 para atermação (jus postulandi), e (3) os PIDs — terminais físicos nos fóruns para quem não tem internet. São jornadas com backstage, processos de suporte e fail points diferentes entre si.

**Resposta recomendada pelo Claude:**
Canal principal (Celeste→Zoom) como swim lane primária, com os canais WhatsApp e PID tratados como fluxos alternativos de entrada em uma faixa lateral anotada — sem desdobrar um blueprint completo para cada um. Rationale: manter os três em profundidade igual explode o artefato; o PID e o WhatsApp são relevantes principalmente como evidência do `[H_Deslocamento_Contraditório]` e do `[H_Gargalo_WhatsApp]`.

**Resposta do usuário:**
> "cobre os três canais de entrada"

**Decisão locked-in:** Três canais em profundidade igual — Web/Celeste→Zoom (A), WhatsApp Atermação (B), PID Físico (C). O usuário optou por cobertura completa em detrimento da recomendação de compactar B e C.

---

### Q3/6 — Tratamento dos marcadores `[H_*]`

**Pergunta formulada:**
> Como tratar os marcadores `[H_*]` no blueprint AS-IS — incluir como fail points "hipotéticos" com notação visual distinta, ou excluir e restringir o artefato apenas às certezas documentais? O v3 estabelece uma Regra Epistêmica Estrita: tudo não verificado vira `[H_*]`. Num blueprint AS-IS puro, só deveriam constar elementos confirmados. Mas excluir todos os `[H_*]` produziria um artefato raso — as camadas de Backstage e Processos de Suporte ficariam quase vazias, e os fail points mais críticos (opacidade da fila, fadiga do servidor, fragmentação PJe/Zoom) desapareceriam.

**Resposta recomendada pelo Claude:**
Incluir os `[H_*]` como fail points hipotéticos com notação visual explícita — célula prefixada com `⚠ [H]` e nota de rodapé explicando o estatuto epistêmico. Rationale: o blueprint serve como instrumento de pesquisa de campo; tornar visíveis as hipóteses orienta diretamente as entrevistas e requisições LAI do Plano de Lacunas, mantendo rastreabilidade entre o artefato e o v3.

**Resposta do usuário:**
> "adicione os fail points sim"

**Decisão locked-in:** Hipóteses `[H_*]` incluídas no blueprint com marcador `⚠ [H_nome]` e símbolo `★FP` para fail points. O blueprint deixa de ser um AS-IS "de certezas" e passa a ser um instrumento híbrido de diagnóstico e pesquisa.

---

### Q4/6 — Mapeamento da camada Normativos e Governança

**Pergunta formulada:**
> A camada "Normativos e Governança" do v3 entra no blueprint como uma 6ª faixa própria ou é absorvida dentro de "Processos de Suporte"? O Shostack canônico tem 5 camadas separadas por 3 linhas divisórias (Interação, Visibilidade, Interação Interna). O v3 adiciona uma 6ª camada `(f) Normativos e Governança` que não tem equivalente direto no modelo — normativos como a Res. CNJ 372/2021 e a Res. CSJT 425/2025 não são processos operacionais executados por pessoas, mas constrangimentos regulatórios que condicionam todo o blueprint.

**Resposta recomendada pelo Claude:**
6ª faixa própria abaixo de Processos de Suporte, intitulada "Normativos e Governança", separada por uma linha pontilhada (não uma linha de interação Shostack). Rationale: misturar normativos com processos de suporte esconde a distinção entre o que o sistema faz e o que o sistema é obrigado a fazer — distinção crítica para identificar gaps de conformidade. Uma faixa separada torna imediatamente visível quando uma etapa não tem normativo associado (lacuna regulatória) ou quando o normativo existe mas o processo não o cumpre (gap de implementação).

**Resposta do usuário:**
> "normativos e governança entra como uma faixa própria"

**Decisão locked-in:** 6ª faixa "Normativos e Governança" separada por "Linha Regulatória" abaixo de Processos de Suporte. Extensão justificada do modelo Shostack para o contexto do serviço público jurisdicional.

---

### Q5/6 — Granularidade das etapas

**Pergunta formulada:**
> As 4 etapas macro do v3 são suficientes, ou o blueprint precisa de sub-etapas para acomodar os três canais? Com três canais confirmados (Celeste→Zoom, WhatsApp atermação, PID físico), os estágios "Descoberta e Triagem" e "Espera e Direcionamento" divergem materialmente por canal — a jornada do PID começa com deslocamento físico até o fórum, a do WhatsApp não passa pela Celeste nem pelo Zoom, e a do canal principal tem a fricção da árvore de decisão da Celeste. Manter 4 colunas únicas força células com conteúdo tripartido e ilegível.

**Resposta recomendada pelo Claude:**
Expandir para 5 etapas, desdobrando "Descoberta e Triagem" em duas colunas: "Pré-acesso / Escolha do Canal" e "Triagem e Direcionamento". As etapas 3 e 4 (Atendimento Síncrono e Pós-Atendimento) convergem nos três canais e podem permanecer unificadas. Rationale: sub-linhas por canal dentro de colunas de etapas únicas criariam células com conteúdo tripartido e ilegível.

**Resposta do usuário:**
> "as 4 etapas são suficientes"

**Decisão locked-in:** 4 etapas macro mantidas — (1) Descoberta e Triagem; (2) Espera e Direcionamento; (3) Atendimento Síncrono; (4) Pós-Atendimento e Encerramento. A divergência entre canais é absorvida pelas sub-linhas A/B/C dentro de cada etapa.

---

### Q6/6 — Representação dos canais no artefato

**Pergunta formulada:**
> Como representar os três canais dentro das 4 etapas — sub-linhas por canal na faixa de Ações do Cidadão, ou uma linha unificada com anotações de divergência? Os três canais divergem nas etapas 1 e 2 mas convergem nas etapas 3 e 4. Com 4 etapas fixas, a única forma de tornar as divergências visíveis sem criar três blueprints separados é estrutural: ou cada canal vira uma sub-linha dentro das faixas que divergem, ou a célula única absorve os três fluxos com anotações textuais.

**Resposta recomendada pelo Claude:**
Sub-linhas por canal nas faixas que divergem (Ações do Cidadão, Frontstage, Evidências Físicas) nas etapas 1 e 2, com fusão das linhas nas etapas 3 e 4 onde os canais convergem. Rationale: anotações textuais dentro de uma célula única criam paredes de texto ilegíveis; sub-linhas preservam a leitura horizontal (a jornada de cada canal) e a leitura vertical (o que acontece simultaneamente em cada etapa), que são as duas leituras analíticas fundamentais do blueprint.

**Resposta do usuário:**
> "pode criar sublinhas por canal e fundir onde eles convergem"

**Decisão locked-in:** Sub-linhas A/B/C em todas as faixas nas etapas 1–2; marcação explícita de *(convergência)* com linha de fusão nas etapas 3–4. A convergência é sinalizada em linha separada dentro de cada faixa para preservar a leitura vertical.

---

## Shared Understanding Reached

Todas as 6 ramificações do decision tree foram resolvidas. O artefato `C_blueprint_asis.md` foi produzido com as seguintes escolhas metodológicas consolidadas:

1. **Persona:** Cidadão leigo hipossuficiente (primária); advogado implícito como secundário
2. **Canais:** A (Web/Celeste→Zoom) + B (WhatsApp Atermação) + C (PID Físico) — cobertura completa
3. **Hipóteses `[H_*]`:** Incluídas como fail points com `⚠ [H_nome]` + `★FP`
4. **Estrutura Shostack:** 6 camadas — Evidências Físicas / Ações do Cidadão / Frontstage / Backstage / Processos de Suporte / Normativos e Governança
5. **Etapas:** 4 macro-etapas — Descoberta e Triagem → Espera e Direcionamento → Atendimento Síncrono → Pós-Atendimento
6. **Layout de canais:** Sub-linhas A/B/C nas etapas 1–2; linha de fusão com *(convergência)* nas etapas 3–4

**13 fail points** mapeados e indexados em `C_blueprint_asis.md`.
