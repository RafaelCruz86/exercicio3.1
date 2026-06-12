Como assistente de pesquisa, estruturei o levantamento das evidências públicas e da arquitetura operacional do **Balcão Virtual do Tribunal Regional do Trabalho da 18ª Região (TRT18 - Goiás)**.

Os achados foram organizados metodologicamente para mapear tanto o fluxo visível quanto os bastidores (*backstage*), as amarras regulatórias e os pontos de fricção latentes, servindo de insumo direto para a construção do seu *Service Blueprint AS-IS*.

---

### MAPEAMENTO DAS EVIDÊNCIAS OPERACIONAIS E REGULATÓRIAS

#### 1. Mapeamento do Processo Operacional Oficial

* **Fonte:** Portal Institucional do TRT18 (trt18.jus.br / Seção de Canais de Atendimento e Balcão Virtual).
* **Tipo de Evidência:** Operacional / Fluxo Oficial.
* **Ator(es) Relacionado(s):** TI / Gestores da plataforma Celeste, Servidores do Balcão Virtual, Cidadãos/Advogados.
* **Trecho-resumo:** O ecossistema de atendimento digital do TRT18 é unificado pela assistente virtual **Celeste** (plataforma *omnichannel*), acessível via chat no portal e WhatsApp. O fluxo inicia-se com uma triagem automatizada (árvore de decisão). Caso a demanda exija intervenção humana ou informações processuais protegidas por segredo de justiça, a Celeste atua como roteadora, direcionando o usuário para os links específicos das salas permanentes do **Zoom** de cada Vara do Trabalho ou unidade administrativa, operando de forma síncrona durante o horário regulamentar de atendimento ao público.
* **Conexão com Hipótese de Fricção (Opacidade da Fila):** A transição entre o ambiente de texto (Celeste) e o ambiente de vídeo (Zoom) carece de um indicador visual de fila de espera unificado. O usuário é inserido em uma "Sala de Espera" no Zoom sem estimativa de tempo ou posição, gerando abandono precoce e percepção de indisponibilidade do serviço.

#### 2. Normativos Aplicáveis (Camada Regulatória)

* **Fonte:** Conselho Nacional de Justiça (Resolução CNJ nº 372/2021); Conselho Superior da Justiça do Trabalho (Resolução CSJT nº 425/2025); Atos Regimentais e Portarias de Teletrabalho do TRT18.
* **Tipo de Evidência:** Normativo / Regulatório.
* **Ator(es) Relacionado(s):** CNJ, CSJT, Magistrados, Presidência/Corregedoria do TRT18.
* **Trecho-resumo:** A Resolução CNJ 372/2021 determina que o Balcão Virtual é de funcionamento obrigatório e síncrono, vedando o agendamento prévio obrigatório como única barreira de acesso. A Resolução CSJT 425/2025 padronizou o **Zoom** como a ferramenta oficial de videoconferência da Justiça do Trabalho, exigindo estabilidade e regras de acessibilidade. No TRT18, os normativos de teletrabalho obrigam as Secretarias de Vara a manter servidores escalados para o monitoramento contínuo da ferramenta durante todo o expediente, sob pena de correição funcional.
* **Conexão com Hipótese de Fricção (Escala Conflitante e Sobrecarga):** Existe uma assimetria entre a cobrança por metas de produtividade internas (bater metas de vazão processual do PJe) e o tempo que o servidor precisa passar "disponível" na tela do Zoom. A escala de balcão concorre diretamente com o trabalho de análise processual de bastidor.

#### 3. Evidências Físicas e de Interface (Backstage e Onstage)

* **Fonte:** Manuais e guias de orientação ao usuário do TRT18; Plataforma de Videoconferência Zoom institucional.
* **Tipo de Evidência:** Evidência física/digital e material de interface.
* **Ator(es) Relacionado(s):** Servidores do Balcão, TI / Gestores da plataforma Celeste.
* **Trecho-resumo:** No *frontstage* (onstage), a evidência é a página centralizadora de links do TRT18, organizada em tabelas com os botões de acesso direto ao Zoom de cada unidade. No *backstage*, a TI gerencia as contas institucionais do Zoom associadas aos e-mails das varas. Os servidores operam em dupla tela: uma mantendo a sessão do Zoom ativa com permissões de *Host/Co-host* para admitir usuários da sala de espera, e outra com o PJe (Processo Judicial Eletrônico) aberto para realizar as consultas em tempo real.
* **Conexão com Hipótese de Fricção (Fracionamento de Telas):** A falta de uma integração nativa API entre a plataforma de vídeo (Zoom), a triagem (Celeste) e o barramento do processo (PJe) força o servidor a realizar consultas manuais e alternar exaustivamente entre janelas, aumentando o tempo médio de atendimento (TMA).

#### 4. Indicadores e Dados de Desempenho

* **Fonte:** Relatório de Gestão Anual do TRT18; Painel de Transparência e Estatísticas (DataJud/CNJ).
* **Tipo de Evidência:** Dado operacional / Métricas de Desempenho.
* **Ator(es) Relacionado(s):** Gestores de Varas/Secretarias, Presidência, CNJ.
* **Trecho-resumo:** Os relatórios estatísticos públicos do Tribunal contabilizam quantitativamente o número de acessos e atendimentos finalizados via Celeste e computam a produtividade geral das secretarias. Contudo, os dados públicos consolidados tratam o atendimento virtual como volumetria agregada, sem discriminar o tempo de resposta nas salas de videoconferência.
* **Conexão com Hipótese de Fricção (Apagão de Métricas de Experiência):** A governança foca em métricas de *output* (quantidade de conexões geradas) e negligencia métricas de *outcome* e experiência (tempo de espera na sala de conferência, taxa de abandono do Zoom e resolução no primeiro contato), ocultando gargalos operacionais crônicos das varas mais demandadas.

#### 5. Fail Points e Vozes Críticas

* **Fonte:** Relatórios Anuais da Ouvidoria do TRT18; Notas de Associações e manifestações da OAB - Seccional Goiás; Estudos sindicais sobre saúde do trabalhador no Judiciário.
* **Tipo de Evidência:** Voz crítica / Relato de falha.
* **Ator(es) Relacionado(s):** Ouvidoria TRT18, OAB-GO, Sindicatos de Trabalhadores.
* **Trecho-resumo:** Advogados relatam episódios de "salas fantasmas": links de Zoom que permanecem ativos, mas com vídeo e áudio desligados por parte do servidor, ou usuários retidos indefinidamente na sala de espera sem qualquer mensagem de previsão. Pelo lado dos servidores, relatórios sindicais apontam o fenômeno do **"Zoom Fatigue"** (exaustão por videoconferência), exacerbado pela pressão de monitorar o balcão simultaneamente ao atendimento de balcão físico e cumprimento de prazos processuais urgentes.
* **Conexão com Hipótese de Fricção (Efeito Fantasma e Fadiga Digital):** O desenho atual do serviço gera uma fricção dupla: o usuário sente-se ignorado em uma interface estática, enquanto o servidor sofre um desgaste de saúde ocupacional devido à dupla exposição síncrona (física e digital) sem suporte psicológico ou pausas estruturadas.

#### 6. Balcão Visual (Libras) e PID (Posto de Informação e Digitação) — Casos de Exclusão

* **Fonte:** Acordos de Cooperação Técnica intertribunais (TRT18 e TRT15); Atos Normativos de Acessibilidade do TRT18; Guia do Usuário dos PIDs.
* **Tipo de Evidência:** Operacional / Mecanismo de Inclusão.
* **Ator(es) Relacionado(s):** Servidores do PID, Intérpretes de Libras (TRT15), Cidadãos em exclusão digital.
* **Trecho-resumo:** O Balcão Visual opera por meio de cooperação técnica em rede judiciária (compartilhamento de intérpretes de Libras com o TRT15) em faixas de horários pré-definidas. Para os cidadãos sem infraestrutura tecnológica, o TRT18 disponibiliza os **PIDs (Postos de Informação e Digitação)** localizados fisicamente nas sedes das Varas e postos avançados no interior do estado de Goiás. O ambiente conta com um terminal de autoatendimento (computador, webcam, scanner) e apoio físico para que o usuário acesse o Balcão Virtual ou envie documentos. O e-mail `sgj@trt18.jus.br` (Secretaria-Geral Judiciária) atua na retaguarda de suporte e governança destes fluxos.
* **Conexão com Hipótese de Fricção (Deslocamento Compulsório / Dependência de Rede):** O PID resolve a exclusão digital, mas gera uma contradição de design: para usar o serviço criado para "evitar deslocamentos", o cidadão hipossuficiente precisa se deslocar fisicamente até o fórum. Além disso, a dependência de intérpretes de outro tribunal (TRT15) fragiliza o SLA caso haja falhas de comunicação ou indisponibilidade técnica na integração entre as regiões.

#### 7. Canal de Atermação

* **Fonte:** Divulgação de Canais de *Jus Postulandi* do TRT18; Núcleo de Atermação e Primeiro Atendimento.
* **Tipo de Evidência:** Operacional / Ponto de contato de entrada.
* **Ator(es) Relacionado(s):** Servidores de Atermação, Cidadãos (Jus Postulandi).
* **Trecho-resumo:** A Atermação (exercício do *Jus Postulandi* sem advogado) possui canal de entrada via WhatsApp dedicado (**62 3222-557062 3222-5570**). O fluxo opera de modo assíncrono: o cidadão envia o relato do caso e imagens de documentos (RG, CPF, CTPS, comprovantes). O servidor da Atermação faz a triagem da matéria trabalhista, analisa a competência territorial e, frequentemente, agenda uma sessão via **Zoom** (articulada com a estrutura do Balcão Virtual) para tomar o depoimento e reduzir a termo a petição inicial.
* **Conexão com Hipótese de Fricção (Gargalo de Legibilidade e Assincronia):** Como o envio de documentos pelo cidadão comum via WhatsApp é desestruturado (fotos tremidas, PDFs incompletos), gera-se um vaivém de mensagens que estende o tempo de atendimento por dias, travando o fluxo na entrada da Atermação antes mesmo de chegar à distribuição processual.

---

### QUADRO SÍNTESE: SERVICE BLUEPRINT AS-IS (BALCÃO VIRTUAL TRT18)

| Camadas do Blueprint | Etapa 1: Descoberta e Triagem | Etapa 2: Espera e Direcionamento | Etapa 3: Atendimento síncrono (Zoom) | Etapa 4: Pós-Atendimento e Encaminhamento |
| --- | --- | --- | --- | --- |
| **(a) Ações do Cliente** | Entra no site do TRT18; clica no ícone da Celeste ou navega na tabela de links; escolhe a unidade desejada. | Clica no link do Zoom da Vara; aguarda a autorização de entrada na tela estática. | Dialoga com o servidor por vídeo/áudio; expõe a dúvida processual; apresenta documento na câmera se solicitado. | Recebe a informação, o número do protocolo ou o link para o PJe; encerra a chamada. |
| **(b) Onstage / Frontstage** | Interface web do Portal TRT18; menu de opções do chatbot Celeste (WhatsApp ou Web). | Mensagem padrão do Zoom: *"Aguarde, o anfitrião da reunião permitirá sua entrada em breve"*. | Interface de vídeo do Zoom institucional; servidor com câmera ligada prestando atendimento humano. | Envio de links/orientações pelo chat do Zoom; encerramento da sessão de vídeo. |
| **(c) Backstage** | Plataforma de triagem omnichannel gerenciando a árvore de automação de mensagens de texto. | Servidor monitora a aba *"Waiting Room"* (Sala de Espera) no Zoom; gerencia a ordem de entrada dos usuários. | Servidor consulta o PJe em uma segunda tela; checa segredo de justiça e identidade; aciona intérprete de Libras via convite se necessário. | Registro interno do atendimento em planilha/sistema de controle; atualização do status na plataforma de atendimento. |
| **(d) Processos de Apoio** | Infraestrutura de TI hospedando o site e a API da Celeste; manutenção dos servidores de chatbot. | Infraestrutura de rede e licenciamento corporativo de contas Zoom gerenciado pela TI do Tribunal. | Banco de dados do PJe (Processo Judicial Eletrônico); barramento de dados do DataJud; sistema de suporte técnico da TI/Celeste. | Sistemas de gestão de estatísticas judiciais; canais internos de comunicação entre a Vara e a Atermação/Ouvidoria. |
| **(e) Evidências Físicas / Digitais** | Portal trt18.jus.br; número de WhatsApp da Celeste; QR codes em cartazes nos fóruns/PIDs. | Tela de espera do aplicativo Zoom; layout da tabela de links do portal do TRT18. | Sala virtual com logo institucional do TRT18; telas de consulta do PJe; formulários digitais de identificação. | Mensagens de texto copiadas e coladas no chat; e-mail de confirmação; links de pesquisas de satisfação (se houver). |
| **(f) Normativos e Governança** | **Res. CNJ 372/2021** (livre acesso sem agendamento); Portarias institucionais de atendimento do TRT18. | **Res. CSJT 425/2025** (padrão Zoom e regras de disponibilidade técnica do canal de vídeo). | Provimento da Corregedoria do TRT18 (escopo do que pode ser informado); regras de sigilo da LGPD aplicadas à justiça. | Metas de produtividade do CNJ; regramento interno de encaminhamento para Ouvidoria ou Distribuição. |

---

### MAPA DE LACUNAS DE INFORMAÇÃO (Foco para LAI e Pesquisa Primária)

Para subsidiar o avanço da pesquisa primária e refinar o diagnóstico de falhas ocultas no *backstage*, mapeou-se o que **não está disponível publicamente** e exige requisição via Lei de Acesso à Informação (LAI) ou exploração direta em entrevistas:

1. **Métricas Ocultas de SLA e Abandono:** Qual é a taxa real de abandono de usuários na sala de espera do Zoom do TRT18? Qual é o tempo médio de espera (TME) real antes de o servidor admitir o usuário na sala de videoconferência? (Estes dados ficam retidos nos relatórios de uso da console administrativa do Zoom corporativo e não constam no DataJud).
2. **Manuais de Contingência de TI:** Existe um protocolo formal de *failover* para o servidor quando a rede de sua residência cai durante o plantão do Balcão Virtual (teletrabalho)? Como a TI do TRT18 monitora se uma sala de videoconferência caiu ou está sem operador ("sala fantasma") em tempo real?
3. **Dados de Saúde Ocupacional (Fadiga Digital):** Existem registros médicos ou pesquisas internas do setor de saúde do TRT18 correlacionando o trabalho em regime de plantão de Balcão Virtual e atendimento concomitante com o aumento de afastamentos por estresse, burnout ou *Zoom Fatigue*?
4. **Estatísticas de Uso do PID e Balcão Visual:** Quantos atendimentos foram realizados nos terminais físicos dos PIDs no último ano? Quantas vezes a cooperação técnica com o TRT15 para tradução de Libras foi efetivamente acionada no Balcão Visual e qual o índice de falha/indisponibilidade desse serviço compartilhado?
5. **Acordo de Nível de Serviço da Atermação:** Qual o tempo médio de resposta (SLA) para a primeira interação humana após o envio dos documentos de reclamação trabalhista no WhatsApp da Atermação (62 3222-5570)?

```
Vou te enviar uma pesquisa que outro assistente de IA produziu sobre a
OPERAÇÃO do Balcão Virtual do TRT18. Faça uma AUDITORIA RIGOROSA.
Identifique TODAS as falhas:
  - erros factuais (cite o trecho)
  - etapas de bastidor (backstage) omitidas
  - evidências físicas ou normativos relevantes que ficaram de fora
  - fail points não identificados
  - inferências mal-suportadas / fontes fracas
NÃO conte como falha questões cosméticas (formatação, estilo, ordem).
Para cada falha, cite o trecho e justifique.
```

---

# claude response

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
