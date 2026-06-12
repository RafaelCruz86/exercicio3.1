# Segunda Auditoria — v2 do Relatório sobre o Balcão Virtual TRT18

## Avaliação geral

A v2 é estruturalmente mais honesta — ela nomeia o jogo (hipótese vs. normativo vs. lacuna) e isso é um ganho real. Mas o padrão de fundo da v1 **se repete**: a v2 continua introduzindo afirmações factuais específicas sem fonte, só que agora "blindadas" por um disclaimer geral no item 0. O disclaimer não imuniza afirmações concretas e novas que aparecem depois dele como se fossem dados. Abaixo, item por item.

---

## (a) Itens do audit_v1 — foram de fato endereçados?

| # | Item v1 | Endereçado? | Observação |
|---|---|---|---|
| 0 | Ausência de URLs/fontes | **Parcialmente.** Reconhece o problema, mas a "solução" é um disclaimer geral — não impede que itens novos da v2 cometam o mesmo erro (ver seção b). |
| 1.1 | Waiting Room como fato | **Sim.** Rebaixado a hipótese H_Fila, com ação de campo definida. Correto. |
| 1.2 | "Salas fantasmas" | **Sim.** Rebaixado a H_Fantasma, com plano de LAI. Correto. |
| 1.3 | Detalhe da Res. CSJT 425/2025 | **Parcialmente, e com problema novo** (ver b.1 abaixo — a correção introduz uma citação normativa nova e não verificada). |
| 1.4 | "Provimento da Corregedoria" inventado | **Sim.** Tratado como lacuna aberta, com origem reconhecida ("foi uma extrapolação analítica"). Bom. |
| 1.5 | Dupla tela / contas Zoom por vara | **Parcialmente.** Reclassificado como "Arquitetura de Referência Operacional Provável" — mas a tabela síntese final volta a apresentar isso como **[H_Telas]** no backstage da Etapa 3 sem reforçar que é hipótese não validada lá. É uma melhoria de rótulo, não de robustez. |
| 2.1 | TI/Celeste — conflito uptime vs. equidade | **Sim**, e bem desenvolvido — agora aponta o funil de triagem da Celeste como barreira de exclusão. Boa adição analítica. |
| 2.2 | OAB-GO — papel duplo | **Sim.** Cobre as duas faces (pressão por estabilidade + resistência à automação). |
| 2.3 | Magistrados / H2 | **Sim**, e é a melhor seção da v2 — conecta corretamente a restrição informacional a risco de nulidade/imparcialidade. |
| 2.4 | Sindicatos como canal oculto | **Sim, mas com problema novo** (ver b.2 — nomeia um sindicato específico sem fonte). |
| 2.5 | STF | **Sim.** Tratado como lacuna aberta, formulação adequada. |
| 2.6 | ANPD/LGPD | **Parcialmente, e com problema novo** (ver b.3 — afirma como "em regra" algo não verificado). |
| 2.7 | Zoom Inc. / SLA | **Sim.** Tratado como lacuna aberta, com plano de LAI. Bom. |
| 2.8 | Gestores de Varas / H4 | **Sim.** Conecta corretamente fadiga + ausência de dashboard de carga. |
| 3 | Evidências físicas ausentes (editais, portarias DEJT, FAQ Celeste) | **Não realmente endereçado — apenas reformulado como lacuna genérica**, exceto a Celeste, que recebeu um problema novo grave (ver b.4). |
| 4 | Fail points novos (sigilo em teletrabalho, autenticação, concorrência Atermação/Balcão) | **Sim**, os três foram incorporados quase literalmente como Fail Points A, B, C. Bem aproveitado. |

---

## (b) Falhas NOVAS introduzidas pela v2

### b.1 — Citação normativa nova e não verificada: "Resolução CNJ nº 401/2021"

> "As exigências de acessibilidade digital e estabilidade sistêmica derivam, na verdade, do plano macrorregulatório do CNJ (notadamente a **Resolução CNJ nº 401/2021**, que trata da acessibilidade para pessoas com deficiência, e as diretrizes do **Prêmio CNJ de Qualidade**)."

Isso é **exatamente o tipo de erro que a auditoria v1 apontou** (item 1.3) — só que agora com um número de resolução específico, citado com confiança, sem qualquer fonte. A v2 *substitui* uma alegação vaga não verificada por uma alegação **mais específica e ainda não verificada**, o que é pior, não melhor: um número de resolução errado tem potencial de contaminar toda a cadeia normativa do blueprint se for citado adiante como se fosse confirmado. Não há indicação de que esse número foi checado contra o texto real do CNJ. Deveria ter sido tratado como lacuna ("há normativos do CNJ sobre acessibilidade que precisam ser identificados"), não como citação nomeada.

### b.2 — "SINJUFREGO" citado como sindicato relevante, sem verificação

> "Os sindicatos de trabalhadores (como o **SINJUFREGO** no âmbito interno e as federações laborais locais no externo)..."

SINJUFREGO é o sindicato de servidores do Judiciário Federal em Goiás — ou seja, representaria os **servidores do TRT18** (operadores), não os usuários vulneráveis (trabalhadores que buscam o Balcão Virtual). O parágrafo trata desse ator como canal de "demanda reprimida dos usuários" (trabalhadores rurais, terceirizados), mas o exemplo nomeado é um sindicato de **servidores públicos**, não de trabalhadores jurisdicionados. Há uma confusão de categoria de ator: o mapa de stakeholders original trata "Sindicatos de Trabalhadores" como vozes dos usuários, e a v2 ilustra esse ator com um sindicato que, na verdade, representaria mais naturalmente os "Servidores do Balcão" (outro ator do mapa). Isso é uma **inferência mal-suportada nova**, do mesmo tipo criticado no item 1.2 do audit_v1 (atribuição de papel a entidade nomeada sem fonte e sem checagem de pertinência).

### b.3 — Afirmação categórica sobre gravação de sessões, sem fonte

> "A gravação das sessões de atendimento do Balcão Virtual é, **em regra, desativada** para mitigar o risco de vazamento e armazenamento indevido, o que por sua vez elimina a principal evidência física em caso de apuração de desvios..."

Essa frase está dentro da seção 2.6, que foi marcada como "(a) Corrigir com texto novo" — ou seja, apresentada como **correção factual**, não como hipótese. Mas não há nenhuma fonte (portaria, política de privacidade, manual) que confirme essa prática. É uma afirmação tão forte e tão específica quanto as que a v1 já havia derrubado (ex.: "salas fantasmas", "Waiting Room"), só que aqui ela não foi rebaixada a hipótese — ao contrário, é usada para sustentar a conclusão de que "elimina a principal evidência física", uma cadeia de raciocínio de dois andares construída sobre uma premissa não verificada. Deveria estar marcada como **[H_Gravação]** ou listada como lacuna ("não há informação pública sobre se as sessões são gravadas e por quanto tempo retidas").

### b.4 — Reconstrução detalhada do menu da Celeste, apresentada como "Retificação v2 / Corrigir com texto novo"

> "As opções iniciais dividem-se de forma corporativa: *1. Advogado / 2. Cidadão / 3. Certidões / 4. Links de Audiências*. O direcionamento [...] exige que o usuário passe por no mínimo três submenus de texto..."

Isso é classificado como "(a) Corrigir com texto novo" — ou seja, apresentado como **a correção/substituição da evidência física que faltava** (item 3 do audit_v1, que pedia exatamente isso: "página/FAQ pública da Celeste... não reproduz nem referencia nenhum conteúdo concreto"). A v2 responde a essa cobrança **inventando o conteúdo do menu** com detalhe (quatro opções numeradas, "no mínimo três submenus"). Isso é uma regressão direta: o audit_v1 pediu evidência real e a v2 entregou uma evidência fabricada com aparência de verificada, na seção que menos deveria admitir isso, porque é justamente sobre uma interface pública que poderia ter sido checada por acesso direto ao site.

### b.5 — Inconsistência entre o disclaimer geral (item 0) e o tratamento diferenciado dos demais itens

A v2 trata alguns itens como "(a) corrigir" + "(c) pendente" (ex.: 1.1, 1.2) — rebaixando a hipótese **e** abrindo lacuna de validação — mas trata outros itens igualmente não verificados (b.1, b.2, b.3, b.4 acima) apenas como "(a) corrigir", sem o "(c) pendente" correspondente. Não há critério explícito para essa diferença. O efeito prático é que as afirmações mais "plausíveis" (gravação desativada, menu da Celeste, resolução do CNJ específica) escapam do mesmo escrutínio aplicado às afirmações mais "vistosas" (salas fantasmas, waiting room) — quando deveriam receber o **mesmo tratamento**, pois o nível de verificação real é o mesmo (zero).

### b.6 — Tabela síntese mistura hipóteses marcadas e não marcadas sem critério consistente

Na tabela final, alguns campos recebem marcadores `[H_Fila]`, `[H_Telas]`, `[H_Escopo]` — mas outros campos igualmente especulativos não recebem marcador algum, por exemplo:

> "(e) Evidências Físicas / Digitais [...] Logotipo institucional configurado como fundo de tela virtual; visualização dos documentos via câmera." (Etapa 3)
> "(f) [...] Regras de descarte e retenção de dados cadastrais em conformidade técnica com a LGPD." (Etapa 4)

Essas afirmações têm o mesmo status epistêmico (inferência plausível não verificada) das que foram marcadas como H_ algo, mas aparecem na tabela como se fossem descrições factuais do AS-IS. Isso reintroduz, na camada que será mais usada (a tabela síntese é o artefato de trabalho do blueprint), a mesma ambiguidade fato/hipótese que a v2 prometeu eliminar.

---

## (c) Pontos que permanecem abertos (não piores, mas ainda não resolvidos)

1. **Nenhuma verificação foi de fato realizada** — a v2 é inteiramente um exercício de reclassificação textual do mesmo conteúdo da v1, sem nenhuma nova consulta a fonte primária (mesmo as que seriam triviais, como acessar o portal trt18.jus.br para ver o menu real da Celeste, o que tornaria b.4 desnecessário).
2. O **Fail Point B (autenticação via webcam)** continua sendo uma inferência sobre "como provavelmente funciona", sem qualquer indicação de que esse é, de fato, o procedimento do TRT18 — está bem formulado como hipótese de risco, mas não está rotulado como tal na nomenclatura H_ usada em outros lugares.
3. A confusão entre **TRT15** (que de fato é sede em Campinas-SP — isso está correto) e o papel dele na cooperação de Libras permanece sem verificação de que esse acordo específico exista; foi corretamente listado como lacuna (item 4 do plano de lacunas), então isso está OK, mas vale registrar que não foi auditado se "TRT15" é mesmo o tribunal correto citado no mapa de atores original (o mapa original já trazia essa informação, então a origem é o próprio insumo, não a pesquisa — isso é aceitável, mas não foi re-verificado).
4. **Critério de "o que vira hipótese vs. o que vira lacuna vs. o que é mantido como fato" não está explicitado como regra geral** — cada item da v2 parece ter recebido um tratamento ad hoc. Isso significa que uma v3 corrigindo b.1–b.4 provavelmente vai, de novo, introduzir novas afirmações específicas não verificadas em outros pontos, a menos que se estabeleça uma regra simples: *toda afirmação sobre conteúdo, número de norma, nome de entidade ou procedimento específico que não veio do mapa de atores original e não tem fonte citável vira automaticamente "[H_x]" ou item do plano de lacunas — sem exceção.*

---

## Síntese

A v2 corrige bem as falhas **estruturais/analíticas** apontadas no audit_v1 (itens 2.1–2.8, que eram sobre atores e hipóteses diagnósticas) — essa parte do trabalho está sólida e bem argumentada. Mas, na tentativa de "preencher" as lacunas de evidência factual e normativa (itens 0, 1.3, 1.5, e especialmente o item 3 sobre evidências físicas), a v2 **repete o erro original em formato mais sutil**: substitui afirmações vagas não verificadas por afirmações específicas não verificadas (um número de resolução, um nome de sindicato, um menu de quatro opções, uma política de gravação). O risco para o projeto é que essas novas especificidades, por parecerem mais "checadas", tenham mais chance de sobreviver sem crítica em uma v3 ou de serem citadas como dado em entrevistas de validação — quando, na prática, têm exatamente o mesmo lastro (nenhum) que "sala fantasma" tinha na v1.
