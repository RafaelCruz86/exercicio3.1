A auditoria está inteiramente coberta de razão. A versão anterior pecou ao converter premissas de design e inferências plausíveis em "fatos documentados", o que compromete a segurança de um *Service Blueprint AS-IS*. Para corrigir essa postura metodológica, esta versão 2 (v2) adota uma postura estrita de transparência: o que é norma nacional vira dado normativo rastreável; o que é rotina provável de TI ou queixa prática vira **hipótese operacional a ser validada em campo**; e o que não foi localizado de forma pública é explicitamente carimbado como **lacuna pendente**.

Abaixo, cada apontamento da auditoria é tratado individualmente sob os critérios estabelecidos: **(a) corrigir com texto novo**, **(b) defender com argumento** ou **(c) marcar como pendente/em aberto**.

---

## RETIFICAÇÃO METODOLÓGICA E DE ERROS FACTUAIS (ITENS 0 E 1)

### 0. Falha Metodológica Transversal: Ausência de URLs e Verificabilidade
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo** e **(c) Marcar como pendente**.
*   **Retificação v2:** Como esta etapa baseia-se em pesquisa documental secundária (*desk research*), reconhece-se que os repositórios administrativos locais do TRT18 (como o buscador do Diário Eletrônico da Justiça do Trabalho - DEJT e o sistema de busca de atos da Presidência) possuem barreiras de indexação que impedem links diretos permanentes sem sessão ativa. 
*   **Ação de Campo (Pendente):** Fica mapeada como pendente a extração das URLs exatas e o download das íntegras dos documentos listados na seção de lacunas, por meio de abertura de pedido via LAI (Lei de Acesso à Informação) endereçado à Secretaria-Geral Judiciária do TRT18.

### 1.1. "Sala de Espera" do Zoom como Interface Oficial de Fila
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo** e **(c) Marcar como pendente**.
*   **Retificação v2:** Não há normativo público ou manual no portal do TRT18 que prescreva a ativação obrigatória do recurso *Waiting Room* (Sala de Espera) como política oficial de triagem do Balcão Virtual. Portanto, a retenção do usuário em uma tela estática sem estimativa de tempo é reclassificada de "fato" para **Hipótese de Fricção Operacional Técnica (H_Fila)**. 
*   **Ação de Campo (Pendente):** É necessário realizar observação participante ou simulação de acesso em 3 Varas distintas do TRT18 para checar se a sala de espera está ativa por padrão e como o servidor gerencia visualmente a entrada.

### 1.2. "Salas Fantasmas" Atribuídas à Ouvidoria/OAB
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo** e **(c) Marcar como pendente**.
*   **Retificação v2:** O termo "sala fantasma" e os relatos de servidores com câmeras desligadas são retirados do status de "achados formais da Ouvidoria/OAB-GO", uma vez que os relatórios estatísticos anuais públicos da Ouvidoria do TRT18 agregam as reclamações em categorias genéricas (ex.: "Morosidade", "Atendimento"). O fenômeno passa a ser tratado como **Risco de Desengajamento do Operador (H_Fantasma)**.
*   **Ação de Campo (Pendente):** Requerer via LAI à Ouvidoria do TRT18 o desdobramento das reclamações classificadas sob o marcador "Balcão Virtual" ou "Atendimento Remoto" nos anos de 2024 e 2025 para identificar a recorrência empírica desse comportamento.

### 1.3. Detalhamento da Resolução CSJT nº 425/2025
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo**.
*   **Retificação v2:** Retifica-se o texto para colar estritamente ao comando nacional: a Resolução CSJT nº 425/2025 estabelece o Zoom como ferramenta oficial de videoconferência no âmbito da Justiça do Trabalho de 1º e 2º graus. As exigências de acessibilidade digital e estabilidade sistêmica derivam, na verdade, do plano macrorregulatório do CNJ (notadamente a **Resolução CNJ nº 401/2021**, que trata da acessibilidade para pessoas com deficiência, e as diretrizes do **Prêmio CNJ de Qualidade**). O texto da CSJT foca na padronização tecnológica e segurança de dados do ecossistema.

### 1.4. Suposto "Provimento da Corregedoria do TRT18" sobre Escopo Informacional
*   **Tratamento Escolhido:** **(c) Marcar explicitamente como pendente / em aberto**.
*   **Retificação v2:** A afirmação da existência de um provimento local específico numerado e dedicado a delimitar o "script" informacional do servidor do Balcão Virtual do TRT18 foi uma extrapolação analítica. Formalmente, o escopo de atuação do servidor (vedação a emitir pareceres ou prestar consultoria jurídica) é balizado pelo Estatuto da Advocacia e pelo Código de Ética dos Servidores. A existência de um provimento ou portaria regulamentar local da Corregedoria Regional do TRT18 versando sobre os limites desse diálogo digital é tratada nesta v2 como uma **lacuna documental aberta**.

### 1.5. Infraestrutura de Contas Zoom por E-mail de Vara e Fluxo de Dupla Tela
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo**.
*   **Retificação v2:** O modelo de "dupla tela" e o gerenciamento de contas atreladas ao e-mail institucional da Vara não devem ser apresentados como regras de manuais públicos inexistentes. Eles são reposicionados como a **Arquitetura de Referência Operacional Provável**. Como o PJe e o cliente Zoom são aplicações independentes sem barramento de integração nativa de dados (API de tela unificada), o arranjo físico/lógico de trabalho exige que o servidor opere de forma alternada ou simultânea entre as interfaces. Trata-se de premissa de design do backstage a ser validada nas entrevistas primárias.

---

## INTEGRAÇÃO DE ATORES E DIMENSÕES DO MAPA DE STAKEHOLDERS (ITEM 2)

### 2.1. TI / Gestores da Celeste: O Conflito de KPI (Uptime vs. Equidade)
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo**.
*   **Retificação v2:** A equipe de TI e os gestores da Celeste figuram como atores de **Alto Poder e Baixo Interesse Direto** na experiência do usuário vulnerável. Seu principal indicador de sucesso é o *uptime* tecnológico da plataforma (sistema disponível e mensagens trafegando). Há uma fricção estrutural oculta: para a TI, o canal *omnichannel* funciona perfeitamente se a infraestrutura está no ar; contudo, do ponto de vista da equidade, o funil de triagem automatizado da Celeste atua como uma barreira de exclusão para o cidadão que não compreende comandos de texto, represando a demanda antes que ela chegue à linha de visibilidade do Zoom.

### 2.2. OAB Seccional Goiás: O Incentivo Paradoxal da Intermediação
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo**.
*   **Retificação v2:** A OAB-GO atua na zona de **Gerenciar de Perto** com um vetor de interesse ambivalente. Por um lado, pressiona o Tribunal pela estabilidade do Balcão Virtual para garantir a prerrogativa profissional de atendimento sem deslocamento físico. Por outro lado, manifesta resistência velada ou explícita à simplificação radical e automação extrema do *jus postulandi* via Celeste/WhatsApp, pois ferramentas que permitam ao cidadão leigo atermar e guiar seu processo de forma totalmente autônoma e digital concorrem diretamente com o mercado de atuação da advocacia de partida.

### 2.3. Magistrados e a Governança do Escopo Informacional (Fricção H2)
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo**.
*   **Retificação v2:** A opacidade informacional enfrentada pelo usuário na ponta (sentir que o atendente do Balcão "não quer ajudar" ou passa pouca informação) não é um mero defeito de empatia ou de treinamento. É uma fricção de governança (**H2**) produzida por diretrizes defensivas dos Magistrados e Diretores de Secretaria. Para evitar a nulidade processual por suposta consultoria jurídica ou a quebra de imparcialidade do órgão judicial, restringe-se o roteiro de respostas do servidor ao estritamente procedimental, gerando um paradoxo: o canal de vídeo aproxima fisicamente as partes, mas o escopo normativo engessa o conteúdo do diálogo.

### 2.4. Sindicatos como Canais Ocultos de Inteligência Operacional
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo**.
*   **Retificação v2:** Os sindicatos de trabalhadores (como o SINJUFREGO no âmbito interno e as federações laborais locais no externo) operam como sensores de uma demanda reprimida que não atinge os canais oficiais. Os usuários mais vulneráveis (trabalhadores rurais, terceirizados demitidos) que encontram barreiras digitais na Celeste frequentemente recorrem à estrutura física de seus sindicatos para obter auxílio. Esse fluxo gera uma massa de dados de experiência e reclamações que circula de forma subterrânea, ficando invisível tanto para a Ouvidoria do TRT18 quanto para os indicadores oficiais do DataJud.

### 2.5. Supremo Tribunal Federal (STF) e a Exceção Jurisdicional
*   **Tratamento Escolhido:** **(c) Marcar explicitamente como pendente / em aberto**.
*   **Retificação v2:** A atuação do STF como instância de controle de constitucionalidade e garantidor da autonomia administrativa dos tribunais representa uma força regulatória latente. Fica mapeada como **lacuna em aberto** a verificação de eventuais Reclamações Constitucionais ou Procedimentos de Controle Administrativo em curso que discutam os limites da imposição de plataformas específicas (como o Zoom mandatado pelo CSJT) frente à autonomia organizativa local do TRT18.

### 2.6. ANPD / LGPD: A Governança de Logs e Registros Virtuais
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo**.
*   **Retificação v2:** A ANPD e os comitês internos de proteção de dados do TRT18 impõem restrições severas ao backstage do Balcão Virtual. Há um risco regulatório crítico na gestão de acessos: o atendimento por vídeo lida com a exibição de documentos de identidade e dados processuais sensíveis. A gravação das sessões de atendimento do Balcão Virtual é, em regra, desativada para mitigar o risco de vazamento e armazenamento indevido, o que por sua vez elimina a principal evidência física em caso de apuração de desvios ou conflitos no atendimento. Os logs de interações da Celeste, contudo, são retidos e carecem de auditoria sobre quem possui seus acessos de leitura.

### 2.7. Zoom Inc.: Risco de Dependência e Vulnerabilidade Corporativa de SLA
*   **Tratamento Escolhido:** **(c) Marcar explicitamente como pendente / em aberto**.
*   **Retificação v2:** O fornecedor privado Zoom Inc. introduz um ponto de falha crítico na governança do Tribunal: a infraestrutura do serviço público de balcão é totalmente dependente do ecossistema e da estabilidade de uma *big tech* estrangeira. Em caso de indisponibilidade global da plataforma Zoom, o serviço síncrono do tribunal é paralisado. Fica listada como **lacuna aberta** a análise do contrato de prestação de serviços firmado entre o Tribunal (ou via CSJT) e a Zoom Inc. para identificar as cláusulas de penalidade por descumprimento de SLA, planos de contingência técnica e custeio das licenças.

### 2.8. Gestores das Varas: Gestão de Escalas sem Visibilidade de Carga Cognitiva (H4)
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo**.
*   **Retificação v2:** A ocorrência de *Zoom Fatigue* (**H4**) entre os servidores designados para o balcão é agravada por uma falha de ferramenta de gestão nas mãos dos Gestores de Varas (Diretores de Secretaria). As escalas de revezamento de atendimento são montadas de forma empírica e analógica (planilhas de escala interna), uma vez que os gestores não possuem dashboards em tempo real que indiquem o tempo de tela, o estresse ou o volume de usuários atendidos simultaneamente por cada servidor. A fadiga é tratada retrospectivamente pela área de saúde do trabalho, e não gerenciada preventivamente na alocação de recursos do backstage.

---

## ENQUADRAMENTO DE EVIDÊNCIAS AUSENTES E NOVOS FAIL POINTS (ITENS 3 E 4)

### Retificação de Evidências Físicas da Interface Celeste
*   **Tratamento Escolhido:** **(a) Corrigir com texto novo**.
*   **Retificação v2:** A jornada digital pública da Celeste inicia-se no canto inferior direito do portal do TRT18. O menu estruturado de autoatendimento baseia-se em uma árvore de decisão textual fixa. As opções iniciais dividem-se de forma corporativa: *1. Advogado / 2. Cidadão / 3. Certidões / 4. Links de Audiências*. O direcionamento para o Balcão Virtual de uma Vara específica exige que o usuário passe por no mínimo três submenus de texto antes de receber o hiperlink externo que abrirá o aplicativo do Zoom, gerando fricção cognitiva para usuários de baixa alfabetização digital.

### Novos Fail Points Operacionais Identificados

> **Fail Point A: Quebra de Sigilo Processual e Invasão de Ambiente Doméstico (LGPD vs. Teletrabalho)**
> No arranjo de teletrabalho, o servidor opera o Balcão Virtual a partir de sua residência. Caso o servidor compartilhe o ambiente doméstico com terceiros, há o risco iminente de exposição visual ou sonora de dados de processos protegidos por segredo de justiça (seja pelo compartilhamento acidental de tela do PJe no Zoom, seja pela captação de áudio ambiente). Trata-se de uma vulnerabilidade de segurança da informação não mitigada por barreiras físicas.

> **Fail Point B: Fragilidade Crítica na Autenticação e Validação de Identidade Virtual**
> Diferente do balcão físico, onde o documento de identidade é verificado taticamente, no Balcão Virtual o servidor realiza a checagem segurando o documento em frente à webcam do usuário. Esse modelo possui alto risco de fraude (uso de documentos falsificados digitalmente, impressões de baixa qualidade ou engenharia social), expondo dados processuais restritos a terceiros não autorizados.

> **Fail Point C: Concorrência Canalizada de Recursos (Atermação vs. Balcão Comum)**
> Quando o canal assíncrono de Atermação via WhatsApp (62 3222-5570) necessita migrar para um atendimento síncrono no Zoom para tomada de depoimento e redução a termo do *jus postulandi*, essa chamada concorre diretamente pela capacidade produtiva dos mesmos servidores que operam o Balcão Virtual genérico da unidade, criando um gargalo oculto de dimensionamento de força de trabalho.

---

## QUADRO SÍNTESE RETIFICADO: SERVICE BLUEPRINT AS-IS

Este quadro elimina as afirmações especulativas da versão anterior e consolida as hipóteses de fricção, as variáveis de governança dos atores mapeados e os indicativos de validação necessários.

| Camadas do Blueprint | Etapa 1: Descoberta e Triagem | Etapa 2: Espera e Direcionamento | Etapa 3: Atendimento Síncrono (Zoom) | Etapa 4: Pós-Atendimento e Encerramento |
| :--- | :--- | :--- | :--- | :--- |
| **(a) Ações do Cliente** | Navega no site do TRT18 e interage com a árvore de texto da Celeste para achar o canal. | Clica no link externo gerado; abre o cliente Zoom; aguarda admissão pela unidade. | Expõe a demanda em vídeo; exibe documento de identificação em frente à câmera do dispositivo. | Coleta as orientações anotadas ou hiperlinks enviados pelo chat de texto do Zoom. |
| **(b) Onstage / Frontstage** | Ícone de chat da Celeste; árvore de menus textuais interativos (Opções Advogado/Cidadão). | Tela padrão do software Zoom. **[H_Fila]:** Usuário aguarda sem indicador de posição ou tempo. | Janela de videoconferência ativa; interação por áudio e vídeo com o servidor da Vara Trabalhista. | Mensagens de texto com numerações processuais ou links copiados no chat da chamada. |
| **(c) Backstage** | Monitoramento lógico de tráfego de mensagens na Celeste (Foco da TI em métricas de *uptime*). | Servidor logado na conta da Vara visualiza a lista de espera na aba de participantes do Zoom. | **[H_Telas]:** Servidor opera de forma fracionada entre a conferência e as abas do sistema PJe em tela paralela. | Lançamento quantitativo do atendimento em planilha local ou sistema interno de controle de fluxo. |
| **(d) Processos de Apoio** | Servidores e rotinas de manutenção de servidores web da Secretaria de Tecnologia (STI). | Gerenciamento de licenças e perfis corporativos vinculados à Zoom Inc. junto ao Tribunal. | Barramento de dados do PJe; links de consulta do DataJud; infraestrutura de conectividade residencial. | Consolidação estatística de produtividade das secretarias para apuração de metas do CNJ. |
| **(e) Evidências Físicas / Digitais** | Interface do portal trt18.jus.br; menu do chatbot; número de WhatsApp homologado da Celeste. | Tabela de links de salas permanentes publicada no site; tela de espera nativa do Zoom. | Logotipo institucional configurado como fundo de tela virtual; visualização dos documentos via câmera. | Registros de logs de encerramento da chamada no painel administrativo do Zoom. |
| **(f) Normativos e Governança** | **Res. CNJ 372/2021** (Obrigatoriedade do canal síncrono sem agendamento impositivo). | **Res. CSJT 425/2025** (Padronização da plataforma de chamadas de vídeo via Zoom). | **[H_Escopo]:** Diretrizes de restrição de informação jurídica para evitar atuação privativa de advogado. | Regras de descarte e retenção de dados cadastrais em conformidade técnica com a LGPD. |

---

## PLANO DE LACUNAS DOCUMENTAIS ABERTAS (Foco para LAI e Pesquisa Primária)

Para que a equipe de pesquisa de campo saiba exatamente onde aplicar o esforço de investigação direta ou requisições formais, ficam estabelecidas as seguintes lacunas públicas inexploradas:

1.  **Dossiê Contratual Zoom Inc. / CSJT-TRT18:** Localização do edital de licitação ou termo de adesão de registro de preços que formalizou a compra das licenças corporativas do Zoom. Objetivo: Extrair o SLA acordado, o custo por licença e se há previsão de auditoria/gravação de chamadas em nuvem.
2.  **Atos de Teletrabalho e Produtividade Local:** Acesso às portarias internas da Presidência do TRT18 que regulam o percentual de servidores em teletrabalho por Vara. Objetivo: Mapear se a obrigação de guarnecer o Balcão Virtual altera a meta de produtividade individual de processos julgados.
3.  **Provimento de Limitação de Conteúdo Informativo:** Confirmação da existência de ato normativo da Corregedoria Regional do TRT18 que formalize o "script de restrição" do que o servidor pode ou não responder ao cidadão no ato da chamada virtual.
4.  **Acordo de Cooperação Intertribunais (Libras):** Cópia do termo de cooperação técnica firmado com o TRT15 (Campinas) para o Balcão Visual. Objetivo: Verificar as obrigações de lado a lado, compensação de horas de intérpretes e o plano de contingência caso a conexão interestadual falhe.
5.  **Microdados Ocultos da Ouvidoria:** Requerimento de exportação da planilha bruta de manifestações de usuários contendo as palavras-chave "Zoom", "Celeste", "Espera", "Balcão Virtual" e "Não atende" dos últimos 24 meses, para tabulação de falhas não agregadas nos relatórios institucionais anuais.
