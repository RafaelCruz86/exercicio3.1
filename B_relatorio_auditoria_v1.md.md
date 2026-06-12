# Auditoria — Pesquisa sobre o Balcão Virtual TRT18

## 0. Falha metodológica transversal (a mais grave)

O prompt original exigia, para cada item, **"Fonte (URL completa, data de publicação/acesso)"**. Em nenhum dos 7 blocos isso aparece. As "fontes" citadas são genéricas e não verificáveis:

> "Portal Institucional do TRT18 (trt18.jus.br / Seção de Canais de Atendimento e Balcão Virtual)"
> "Relatório de Gestão Anual do TRT18; Painel de Transparência e Estatísticas (DataJud/CNJ)"
> "Relatórios Anuais da Ouvidoria do TRT18; Notas de Associações e manifestações da OAB - Seccional Goiás"

Não há um único link, número de documento, data ou trecho citado de fato. Isso sugere que o conteúdo foi **gerado por inferência/conhecimento geral sobre como tribunais costumam operar**, e não por pesquisa real no site do TRT18, no CNJ ou em relatórios da Ouvidoria. Isso é uma falha de fundo — não cosmética — porque o produto inteiro se apresenta como "evidências públicas" quando na verdade é especulação plausível.

---

## 1. Erros factuais / afirmações inventadas apresentadas como fato

**1.1 — "Sala de Espera" do Zoom como mecanismo oficial de fila**
> "o usuário é inserido em uma 'Sala de Espera' no Zoom sem estimativa de tempo ou posição, gerando abandono precoce"

Não há nenhuma fonte que comprove que o TRT18 usa o recurso *Waiting Room* do Zoom como interface oficial de fila do Balcão Virtual. É uma inferência genérica sobre "como o Zoom funciona", apresentada como descrição factual do serviço. Isso é central para a hipótese de "opacidade da fila" do blueprint — apoiar uma hipótese diagnóstica em um detalhe técnico não verificado é grave.

**1.2 — "Salas fantasmas" como achado da Ouvidoria/OAB**
> "Advogados relatam episódios de 'salas fantasmas': links de Zoom que permanecem ativos, mas com vídeo e áudio desligados [...]"

Nenhuma fonte real é citada (relatório, notícia, ofício). O termo "sala fantasma" não aparece em nenhum lugar do mapa de atores original nem foi atribuído a uma fonte. Parece ter sido **inventado para preencher a seção "fail points e vozes críticas"**, que é justamente a seção mais sensível porque deveria conter evidência empírica de reclamação real.

**1.3 — Conteúdo detalhado da Resolução CSJT 425/2025**
> "A Resolução CSJT 425/2025 padronizou o Zoom como a ferramenta oficial [...] exigindo estabilidade e regras de acessibilidade."

O mapa de atores original já indicava que a Res. 425/2025 "mandatou migração para Zoom", mas os detalhes adicionais ("exigindo estabilidade e regras de acessibilidade") não têm fonte — são uma extrapolação não verificada do conteúdo normativo. Não há confirmação de que a pesquisa tenha de fato lido o texto da resolução.

**1.4 — "Provimento da Corregedoria do TRT18 (escopo do que pode ser informado)"** (na tabela síntese, etapa 3, camada "Normativos")
Esse item aparece **do nada na tabela final** — não há nenhum bloco de evidência no corpo do texto que sustente a existência desse provimento específico. É uma inferência derivada do mapa de atores (que menciona "Magistrados definem escopo informacional dos servidores" como hipótese, não como normativo confirmado), mas a pesquisa o trata como documento normativo real e nomeado.

**1.5 — "TI gerencia as contas institucionais do Zoom associadas aos e-mails das varas" / fluxo de dupla tela (Zoom + PJe)**
Apresentado como descrição operacional factual do backstage, sem qualquer fonte (manual interno, portaria, entrevista). É plausível, mas é **inferência genérica sobre rotina de atendimento público em tribunais**, não evidência coletada sobre o TRT18 especificamente.

---

## 2. Atores e dimensões do mapa de stakeholders que ficaram de fora ou foram tratados superficialmente

**2.1 — Equipe de TI/Celeste como ator de "Alto Poder / Baixo Interesse" com KPI de uptime conflitante com equidade**
Esse é o **gargalo latente central** do mapa de atores (Passo 2 e Lacuna 1: "TI acredita que a Celeste funciona bem porque uptime é alto"). A pesquisa entregue trata a TI apenas como mantenedora de infraestrutura ("Infraestrutura de TI hospedando o site e a API da Celeste") — não investiga, nem aponta como lacuna, a existência de metas de uptime, indicadores internos de TI ou o conflito entre "sistema está de pé" vs "usuário foi atendido". O bloco 4 (Indicadores) menciona genericamente "métricas de output vs outcome", mas não conecta isso ao ator TI/Celeste especificamente, que é onde o mapa original coloca a tensão.

**2.2 — OAB Goiás como intermediário com incentivo paradoxal**
O mapa de atores trata a OAB-GO em **duas dimensões**: (a) voz crítica que questiona o jus postulandi digital, e (b) interesse estrutural da advocacia na complexidade processual (Passo 3, "Gerenciar de Perto" com nota de incentivo paradoxal). A pesquisa só cobre (a), na seção 5, como crítica genérica. A dimensão (b) — que é a mais relevante para entender *resistência institucional a simplificações* — está ausente.

**2.3 — Magistrados como definidores de escopo informacional dos servidores (H2)**
O mapa de atores trata isso como hipótese diagnóstica central: "fricção H2 (opacidade da fila) é parcialmente produzida por decisão de escopo, não só por design da interface". A pesquisa cita "Magistrados" apenas na linha de governança da tabela síntese, sem desenvolver essa hipótese como fail point — ou seja, atribui a opacidade da fila inteiramente a um problema de UX/Zoom (item 1.1), ignorando a causa institucional apontada pelo próprio mapa fornecido como insumo.

**2.4 — Sindicatos e o canal de feedback subutilizado**
O mapa de atores aponta uma lacuna específica: "dados de reclamação e demanda reprimida dos usuários vulneráveis existem mas não chegam sistematicamente ao DataJud nem à Ouvidoria" (Sindicatos, Passo 5, item 8). A pesquisa menciona "estudos sindicais sobre saúde do trabalhador" apenas para sustentar o "Zoom Fatigue" dos servidores — não trata os Sindicatos como canal de *intelligence* sobre a experiência dos usuários vulneráveis, que é o ângulo que o mapa pede.

**2.5 — STF (exceção jurisdicional à Res. 372/2021)**
Listado explicitamente no mapa de atores como ator de "Manter Satisfeito" com nota "Normativo (potencial)". Não aparece em nenhum lugar da pesquisa — nem mesmo para dizer que não há informação pública sobre isso (o que seria aceitável como "lacuna").

**2.6 — ANPD / LGPD como ator normatizador específico**
O mapa de atores trata a ANPD como ator independente ("Conformidade LGPD para dados dos atendimentos e logs da Celeste"). A pesquisa só menciona "regras de sigilo da LGPD" genericamente na tabela síntese, sem tratar a ANPD como ator de governança com possível fricção sobre **gravações de videochamadas, logs da Celeste e retenção de dados de atendimento** — que é um fail point potencial relevante (ex.: o que acontece com a gravação Zoom de um atendimento? quem tem acesso?).

**2.7 — Zoom Inc. como fornecedor único / risco de SLA**
Listado no mapa como ator próprio ("risco de variação de SLA"). A pesquisa usa o Zoom como pano de fundo operacional em todos os blocos, mas nunca trata **a dependência de um fornecedor privado único** como um fail point de governança (o que acontece se o Zoom tiver outage global? há plano de contingência/fornecedor alternativo? há cláusula contratual de SLA visível em editais/contratos do TRT18?). Essa é uma lacuna de pesquisa real e verificável (contratos públicos de licitação são documentos públicos) que não foi nem buscada nem sinalizada como lacuna.

**2.8 — Gestores das Varas e a lacuna de "carga cognitiva em tempo real" (H4)**
O mapa de atores aponta que "Zoom Fatigue (H4) é invisível para quem define quem atende quando" e propõe um "dashboard de carga cognitiva" como alavanca. A pesquisa menciona Zoom Fatigue (bloco 5) mas não conecta isso à ausência de instrumento de gestão para os Gestores das Varas — trata a fadiga como problema de saúde ocupacional isolado, não como problema de **gestão de escalas sem dado**, que é o enquadramento do mapa original.

---

## 3. Evidências físicas/normativas relevantes ausentes

- **Editais/contratos de licitação do TRT18 com a Zoom Inc.** — documento público real, não buscado, que poderia revelar SLA contratual, escopo de gravação, e custo — relevante tanto para fail points quanto para "evidências físicas/normativas".
- **Atos normativos específicos sobre o Balcão Visual (Libras)** — a pesquisa fala de "Acordos de Cooperação Técnica" e "Atos Normativos de Acessibilidade" de forma genérica, mas não tenta localizar o ato específico que define o horário 12h-16h (já presente no mapa de atores como dado conhecido) nem verifica se esse horário está formalmente publicado em algum lugar — ou seja, não tenta validar uma informação que o próprio mapa de atores já trouxe.
- **Resoluções/portarias de teletrabalho do TRT18** — citadas genericamente ("Atos Regimentais e Portarias de Teletrabalho do TRT18") sem número, data ou conteúdo específico, quando esse é exatamente o tipo de documento público localizável (portarias de tribunais são publicadas no Diário Eletrônico da Justiça do Trabalho - DEJT).
- **Página/FAQ pública da Celeste** — a pesquisa afirma a existência de "manuais e guias de orientação ao usuário" mas não reproduz nem referencia nenhum conteúdo concreto desses materiais (texto de tela, opções do menu, prints).

---

## 4. Fail points não identificados

- **Conflito entre sigilo/segredo de justiça e atendimento por vídeo em ambiente não controlado**: o servidor em teletrabalho atende por Zoom de casa — há risco de exposição de dados processuais sigilosos (tela compartilhada do PJe, áudio em ambiente doméstico) a terceiros presentes no recinto do servidor. Isso é um fail point de governança/LGPD que decorre diretamente do modelo "teletrabalho + Zoom + PJe" descrito pela própria pesquisa, mas que ela não percebe como risco.
- **Dependência de identidade/autenticação no Zoom**: como o servidor confirma a identidade do usuário em uma videochamada (sem documento físico, sem certificado digital)? A pesquisa menciona "apresenta documento na câmera se solicitado" (tabela, etapa 3) mas não trata isso como fail point de fraude/erro de identificação — relevante para um serviço que substitui atendimento presencial com apresentação de documentos.
- **Continuidade entre Atermação e Balcão Virtual**: a pesquisa diz que a Atermação "frequentemente agenda uma sessão via Zoom articulada com a estrutura do Balcão Virtual", mas não explora se essa "articulação" tem fila própria, prioridade, ou se compete pelos mesmos recursos (servidores, salas) do Balcão Virtual comum — um possível ponto de conflito de capacidade não mapeado.

---

## 5. Inferências mal-suportadas / fontes fracas (resumo)

| Trecho | Problema |
|---|---|
| "Sala de Espera... sem estimativa de tempo ou posição" | Apresentado como fato operacional verificado; é suposição sobre comportamento padrão do Zoom |
| "salas fantasmas" relatadas por advogados | Termo e episódio sem fonte, na seção que mais precisava de fonte real |
| "Provimento da Corregedoria... escopo do que pode ser informado" | Surge sem evidência no corpo, tratado como normativo nomeado na tabela |
| Detalhamento da Res. CSJT 425/2025 | Conteúdo específico (acessibilidade, estabilidade) sem citação do texto normativo |
| "TI gerencia contas institucionais do Zoom por e-mail de vara" / fluxo de dupla tela | Inferência genérica sobre rotina de atendimento, sem manual/portaria citado |
| Todas as "Fontes" do documento | Nenhuma URL, data ou identificação documental — viola explicitamente o formato pedido |

---

## Síntese

A estrutura do documento (organização por blocos, conexão com hipóteses, quadro síntese por camada de blueprint) segue corretamente o formato solicitado. O problema de fundo é que **o conteúdo não tem lastro em pesquisa real** — não há uma única citação verificável — e, por isso, tende a reproduzir e generalizar o que já estava no mapa de atores fornecido como insumo, além de preencher lacunas com inferências plausíveis sobre "como tribunais costumam funcionar" (Zoom Waiting Room, dupla tela, etc.), algumas das quais foram apresentadas como achados factuais. Além disso, dimensões centrais do próprio mapa de atores — especialmente o conflito de KPI da TI/Celeste (uptime vs. equidade), o papel duplo da OAB-GO, e a hipótese H2 sobre Magistrados/escopo informacional — não foram exploradas, apesar de serem exatamente as hipóteses diagnósticas mais relevantes para o propósito de equidade definido no Passo 0 do mapa.
