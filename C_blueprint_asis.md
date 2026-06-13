# Service Blueprint AS-IS — Balcão Virtual TRT18

**Metodologia:** Shostack (Evidências Físicas → Ações do Cidadão → Frontstage → Backstage → Processos de Suporte) + 6ª faixa de Normativos e Governança  
**Persona primária:** Cidadão leigo hipossuficiente  
**Canais mapeados:** (A) Web/Celeste → Zoom · (B) WhatsApp Atermação · (C) PID Físico  
**Estatuto epistêmico:** Células marcadas com `⚠ [H_nome]` representam hipóteses operacionais não verificadas documentalmente — alvos prioritários de pesquisa de campo e LAI. Fonte: `B_relatorio_assistente_v3.md`.

---

## Legenda

| Símbolo | Significado |
| :--- | :--- |
| `⚠ [H_nome]` | Hipótese operacional — não confirmada documentalmente |
| `★ FP` | Fail point identificado |
| *(convergência)* | Canais A, B e C fundem-se nesta etapa; conteúdo indicado abaixo |
| **A** | Canal Web / Celeste → Zoom |
| **B** | Canal WhatsApp Atermação (62 3222-5570) |
| **C** | Canal PID Físico (terminais nos fóruns) |

---

## Linhas Divisórias (Shostack)

| Linha | Separa |
| :--- | :--- |
| **Linha de Interação** | Ações do Cidadão ↔ Frontstage (limite do encontro de serviço) |
| **Linha de Visibilidade** | Frontstage (visível ao cidadão) ↔ Backstage (invisível) |
| **Linha de Interação Interna** | Backstage ↔ Processos de Suporte |
| **Linha Regulatória** *(extensão)* | Processos de Suporte ↔ Normativos e Governança |

---

## Blueprint Principal

| Faixa | Canal | Etapa 1 · Descoberta e Triagem | Etapa 2 · Espera e Direcionamento | Etapa 3 · Atendimento Síncrono | Etapa 4 · Pós-Atendimento e Encerramento |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **EVIDÊNCIAS FÍSICAS** | **A** | Interface trt18.jus.br; widget/ícone de chat da Celeste; submenus textuais de triagem `⚠ [H_Interface_Celeste]` ★FP | Hiperlink bruto para sala Zoom permanente da Vara; tela estática de Waiting Room sem indicador de fila, posição ou tempo `⚠ [H_Fila]` ★FP | *(convergência — ver abaixo)* | *(convergência — ver abaixo)* |
| | **B** | Número 62 3222-5570 publicado no portal trt18.jus.br e em cartazes nos fóruns | Mensagens de ida e volta no WhatsApp; pedidos de reenvio de documentos ilegíveis ou incompletos `⚠ [H_Gargalo_WhatsApp]` ★FP | *(convergência)* | *(convergência)* |
| | **C** | Terminal físico (computador + webcam + teclado) nos postos avançados/fóruns; sinalização visual do PID no ambiente | Monitor do terminal PID exibindo Waiting Room do Zoom; servidor PID presente ao lado do cidadão | *(convergência)* | *(convergência)* |
| | *(Etapas 3–4: convergência dos canais)* | — | — | Janela de vídeo Zoom ativa com atendente humano; `⚠ [H_Fundo_Visual]` fundo virtual c/ logotipo TRT18; `⚠ [H_Autenticacao]` documento físico exibido na webcam ★FP; `⚠ [H_Telas]` PJe em tela paralela ★FP | Chat de texto Zoom com links, números de processo e orientações colados pelo servidor; logs de duração da chamada no console administrativo Zoom |
| | | | | | |
| **══ LINHA DE INTERAÇÃO ══** | | | | | |
| | | | | | |
| **AÇÕES DO CIDADÃO** | **A** | Acessa trt18.jus.br; abre chat da Celeste; navega sequência de submenus textuais para localizar o Balcão Virtual `⚠ [H_Interface_Celeste]` ★FP — risco de abandono por analfabetismo funcional/digital | Clica no hiperlink da sala Zoom; aguarda na Waiting Room sem feedback de posição ou tempo estimado `⚠ [H_Fila]` ★FP; risco de abandono precoce do canal `⚠ [H_Fantasma]` ★FP | *(convergência — ver abaixo)* | *(convergência — ver abaixo)* |
| | **B** | Localiza número de WhatsApp; inicia conversa descrevendo demanda trabalhista em linguagem livre | Envia fotos/PDFs de documentos (RG, CTPS, contrato); aguarda resposta assíncrona `⚠ [H_Gargalo_WhatsApp]` ★FP — ciclo de correções pode estender-se por dias | *(convergência)* | *(convergência)* |
| | **C** | Desloca-se fisicamente até o fórum/posto avançado `⚠ [H_Deslocamento_Contraditório]` ★FP; opera terminal com auxílio do servidor do PID | Com auxílio do servidor PID, acessa link Zoom no terminal; aguarda na Waiting Room | *(convergência)* | *(convergência)* |
| | *(Etapas 3–4: convergência dos canais)* | — | — | Expõe demanda por voz e vídeo; exibe documento de identidade na câmera `⚠ [H_Autenticacao]` ★FP; recebe orientações orais e textuais do servidor | Lê/copia orientações e links do chat Zoom; encerra a chamada; busca a próxima etapa processual com base nas informações recebidas |
| | | | | | |
| **══ LINHA DE VISIBILIDADE ══** | | | | | |
| | | | | | |
| **FRONTSTAGE** | **A** | Respostas automatizadas da Celeste; menu de opções gerado pelo chatbot; link para sala Zoom da Vara ao término da triagem | Tela estática do Zoom Waiting Room — sem elemento humano visível, sem indicador de posição ou fila `⚠ [H_Fila]` ★FP | *(convergência — ver abaixo)* | *(convergência — ver abaixo)* |
| | **B** | Mensagem automática de boas-vindas do WhatsApp Business (ou recepção humana direta, não verificado) | Mensagem de acuse de recebimento / solicitação de complementação de documentos (humano ou automático, não verificado) | *(convergência)* | *(convergência)* |
| | **C** | Servidor PID orienta o cidadão presencialmente no terminal; facilita acesso à Celeste ou link direto Zoom | Servidor PID permanece ao lado durante a espera na Waiting Room; medeia comunicação com a Secretaria da Vara | *(convergência)* | *(convergência)* |
| | *(Etapas 3–4: convergência dos canais)* | — | — | Janela de vídeo do servidor humano da Secretaria da Vara do Trabalho; chat de texto do Zoom disponível para orientações escritas | Servidor cola no chat Zoom informações finais, links e orientações; encerra a chamada ou retorna à Waiting Room para o próximo usuário |
| | | | | | |
| **── LINHA DE INTERAÇÃO INTERNA ──** | | | | | |
| | | | | | |
| **BACKSTAGE** | **A** | Lógica de roteamento e árvore de decisão da Celeste configurada pela TI; nenhum servidor humano envolvido nesta etapa | Servidor da Vara monitora aba Waiting Room no painel do operador Zoom; decide manualmente quando admitir cada usuário `⚠ [H_Fantasma]` ★FP — salas podem estar sem operador ativo ou com câmera/microfone desligados | *(convergência — ver abaixo)* | *(convergência — ver abaixo)* |
| | **B** | Servidor designado monitora fila do WhatsApp Business; realiza triagem manual das demandas recebidas | Servidor analisa documentos enviados; solicita correções; pode agendar chamada Zoom para colher depoimento `⚠ [H_Concorrência_Recursos]` ★FP — a chamada disputa as mesmas salas do Balcão Virtual | *(convergência)* | *(convergência)* |
| | **C** | Servidor PID opera junto ao cidadão; verifica disponibilidade da sala Zoom da Vara correspondente | Servidor PID coordena com a Secretaria da Vara; servidor da Vara monitora Waiting Room | *(convergência)* | *(convergência)* |
| | **[Balcão Visual — Libras]** | — | Intérprete de Libras cedido pelo TRT15 (Campinas) acionado sob demanda `⚠ [H_SLA_Rede]` ★FP | `⚠ [H_SLA_Rede]` ★FP | — |
| | *(Etapas 3–4: convergência dos canais)* | — | — | Servidor alterna manualmente entre Zoom e PJe para consultar andamentos processuais em tempo real `⚠ [H_Telas]` ★FP; `⚠ [H_Escopo]` restringe diálogo a andamentos para evitar nulidade processual; `⚠ [H_Segredo_Teletrabalho]` risco de exposição de dados sigilosos em ambiente doméstico ★FP; `⚠ [H_Fadiga_Digital]` esgotamento por monitoramento síncrono contínuo ★FP | Registro do atendimento concluído em planilha ou formulário local de controle da Vara `⚠ [H_Apagão_Métricas]` ★FP |
| | | | | | |
| **PROCESSOS DE SUPORTE** | **A** | Infraestrutura de servidores web da STI; sistema de automação da Celeste; provedor de hospedagem do portal trt18.jus.br | Licenciamento corporativo Zoom Inc. `⚠ [H_SLA_Fornecedor]` ★FP — dependência exclusiva de infraestrutura proprietária estrangeira; salas permanentes provisionadas pela STI | *(convergência — ver abaixo)* | *(convergência — ver abaixo)* |
| | **B** | Conta corporativa WhatsApp Business do TRT18; armazenamento temporário de mensagens recebidas | Infraestrutura WhatsApp Business; armazenamento e tráfego de mídias (fotos, PDFs) | *(convergência)* | *(convergência)* |
| | **C** | Infraestrutura física dos PIDs (hardware, rede, manutenção); suporte técnico da STI aos terminais | Conectividade institucional do PID; licença Zoom vinculada ao terminal PID | *(convergência)* | *(convergência)* |
| | *(Etapas 3–4: convergência dos canais)* | — | — | Banco de dados do PJe (Processo Judicial Eletrônico); infraestrutura de conectividade residencial dos servidores em teletrabalho; servidores Zoom Inc.; `⚠ [H_Gravacao]` política de armazenamento e descarte das gravações das chamadas | `⚠ [H_Apagão_Métricas]` Consolidação estatística focada em uptime técnico e volume de chamadas encerradas; ausência de indicadores de outcome: taxa de abandono na Waiting Room, tempo médio de espera, índice de resolução no primeiro contato |
| | | | | | |
| **·· LINHA REGULATÓRIA ··** | | | | | |
| | | | | | |
| **NORMATIVOS E GOVERNANÇA** | **A** | **Res. CNJ nº 372/2021** — obrigatoriedade do Balcão Virtual em todos os tribunais; funcionamento síncrono idêntico ao horário presencial; vedação ao agendamento prévio como barreira única de acesso | **Res. CSJT nº 425/2025** — adoção mandatória do Zoom como plataforma de videoconferência oficial; **Res. CNJ nº 372/2021** — vedação ao agendamento como barreira | *(convergência — ver abaixo)* | *(convergência — ver abaixo)* |
| | **B** | **Res. CNJ nº 372/2021** (acesso amplo); `⚠ sem normativo verificado específico para o canal WhatsApp Atermação` | `⚠ sem normativo verificado` para este canal nesta etapa | *(convergência)* | *(convergência)* |
| | **C** | **Res. CNJ nº 372/2021** — PIDs como mecanismo de inclusão digital e acesso ao serviço | **Res. CNJ nº 372/2021** | *(convergência)* | *(convergência)* |
| | *(Etapas 3–4: convergência dos canais)* | — | — | **Res. CSJT nº 425/2025**; `⚠ [H_Macroregulação]` normativos CNJ de acessibilidade digital — número e teor exatos pendentes de verificação; `⚠ [H_Controle_LGPD]` diretrizes de gravação e LGPD; `⚠ [H_Escala_Concorrente]` portarias de teletrabalho TRT18 — tempo no Balcão computa na meta de produtividade do servidor? | `⚠ [H_Controle_LGPD]` diretrizes de descarte ou proibição de gravação de chamadas em nuvem — não verificado |

---

## Fail Points Consolidados

| ID | Hipótese | Etapa | Canal | Impacto no Cidadão |
| :--- | :--- | :--- | :--- | :--- |
| FP-01 | `[H_Interface_Celeste]` | 1 | A | Funil de exclusão por analfabetismo funcional/digital na triagem da Celeste |
| FP-02 | `[H_Deslocamento_Contraditório]` | 1 | C | Cidadão sem internet desloca-se ao fórum para usar serviço projetado para eliminar o deslocamento |
| FP-03 | `[H_Fila]` | 2 | A, C | Waiting Room sem indicador de posição/tempo induz abandono precoce do canal |
| FP-04 | `[H_Fantasma]` | 2 | A | Sala Zoom publicada no portal sem operador humano ativo — cidadão espera indefinidamente |
| FP-05 | `[H_Gargalo_WhatsApp]` | 2 | B | Ciclo de reenvio de documentos ilegíveis estende o processo de atermação por dias |
| FP-06 | `[H_Concorrência_Recursos]` | 2 | B | Migração do WhatsApp para Zoom disputa capacidade das mesmas salas e servidores do Balcão Virtual |
| FP-07 | `[H_Autenticacao]` | 3 | Todos | Validação de identidade por exibição de documento na webcam — suscetível a fraudes e falsificações |
| FP-08 | `[H_Telas]` | 3 | Todos | Servidor alterna manualmente entre Zoom e PJe sem integração — latência e risco de erro de informação |
| FP-09 | `[H_Fadiga_Digital]` | 3 | Todos | Esgotamento cognitivo pelo monitoramento síncrono contínuo degrada a qualidade do atendimento |
| FP-10 | `[H_Segredo_Teletrabalho]` | 3 | Todos | Dados processuais sigilosos expostos em ambiente doméstico do servidor em teletrabalho |
| FP-11 | `[H_SLA_Fornecedor]` | 2–3 | A, C | Interrupção global do Zoom paralisa todo o atendimento síncrono sem redundância |
| FP-12 | `[H_SLA_Rede]` | 2–3 | Todos | Falha na coordenação interestadual TRT18–TRT15 compromete atendimento a pessoas com deficiência auditiva |
| FP-13 | `[H_Apagão_Métricas]` | 4 | Todos | Ausência de métricas de outcome torna a exclusão digital invisível para a gestão |

---

## Referências

- Fonte primária: `B_relatorio_assistente_v3.md`
- Normativos verificados: Res. CNJ nº 372/2021; Res. CSJT nº 425/2025
- Plano de validação das hipóteses: seção "Plano de Lacunas Documentais Abertas" em `B_relatorio_assistente_v3.md`
- Metodologia: SHOSTACK, G. L. "How to Design a Service." *European Journal of Marketing*, 1982.
