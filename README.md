# Exercício 3.1 — Service Blueprint AS-IS: Balcão Virtual TRT18

**Autor:** Rafael Monteiro da Cruz

Análise e modelagem do serviço de atendimento digital do Tribunal Regional do Trabalho da 18ª Região (TRT18), produzida em ciclos iterativos de pesquisa, auditoria epistêmica e co-design assistido por IA.

---

## Contexto

O **Balcão Virtual** é o canal de atendimento por videochamada (Zoom) do TRT18, criado para fornecer informações processuais sem deslocamento ao fórum. O exercício mapeia o estado atual (AS-IS) do serviço segundo a metodologia de **Service Blueprint de Shostack**, com foco na persona primária do **cidadão leigo hipossuficiente**.

Três canais foram mapeados em profundidade igual:

| Sigla | Canal |
| :--- | :--- |
| **A** | Web / Celeste → Zoom |
| **B** | WhatsApp Atermação (62 3222-5570) |
| **C** | PID Físico (terminais nos fóruns) |

---

## Metodologia

O blueprint segue as **6 faixas de Shostack** (Evidências Físicas → Ações do Cidadão → Frontstage → Backstage → Processos de Suporte) acrescidas de uma **6ª faixa de Normativos e Governança** (CNJ 372/2021, CSJT 425/2025 e portarias internas do TRT18).

Células marcadas com `⚠ [H_nome]` representam hipóteses operacionais não verificadas documentalmente — alvos prioritários de pesquisa de campo e pedidos via LAI. Essa distinção epistêmica foi consolidada a partir da **v3 do relatório de evidências**, que adota a Regra Epistêmica Estrita: apenas dados com fonte pública verificável recebem status de certeza; todo o restante é explicitamente rebaixado a hipótese.

As decisões metodológicas sobre persona, escopo de canais, granularidade de etapas e representação do artefato foram definidas em sessão estruturada de **Grill-Me** e estão registradas em `grill_transcript.md`.

---

## Artefatos

| Arquivo | Etapa | Descrição |
| :--- | :--- | :--- |
| [meta_prompt.md.md](meta_prompt.md.md) | Orientação | Meta-prompt que instrui o assistente de deep research a levantar evidências públicas sobre o Balcão Virtual |
| [relatorio_assistente_v1.md](relatorio_assistente_v1.md) | Pesquisa | Relatório de evidências v1 — levantamento inicial (contém imprecisões documentadas na auditoria v1) |
| [relatorio_auditoria_v1.md](relatorio_auditoria_v1.md) | Auditoria | Auditoria v1 — identificação de erros e inconsistências do relatório inicial |
| [relatorio_assistente_v2.md](relatorio_assistente_v2.md) | Pesquisa | Relatório de evidências v2 — primeira revisão após auditoria v1 |
| [relatorio_auditoria_v2.md](relatorio_auditoria_v2.md) | Auditoria | Auditoria v2 — segunda rodada de checagem epistêmica |
| [relatorio_assistente_v3.md](relatorio_assistente_v3.md) | Pesquisa | Relatório de evidências v3 — versão saneada com Regra Epistêmica Estrita e marcadores `[H_*]` |
| [grill_transcript.md](grill_transcript.md) | Co-design | Transcript da sessão Grill-Me — 6 decisões metodológicas locked-in |
| [blueprint_asis.md](blueprint_asis.md) | Artefato | Service Blueprint AS-IS completo (6 camadas Shostack, 3 canais, 13 fail points) |
| [diagrama_asis.md](diagrama_asis.md) | Artefato | Diagrama Mermaid das relações entre etapas, atores e fail points |

---

## Decisões Metodológicas (Grill-Me)

| # | Decisão | Definição |
| :--- | :--- | :--- |
| 1 | Persona primária | Cidadão leigo hipossuficiente |
| 2 | Escopo de canais | Três canais em profundidade igual: A + B + C |
| 3 | Tratamento de `[H_*]` | Incluir como fail points com notação `⚠ [H_nome]` + `★FP` |
| 4 | Camada de Normativos | 6ª faixa própria, separada por linha regulatória |
| 5 | Granularidade | 4 etapas macro (Descoberta, Espera, Atendimento, Pós-Atendimento) |
| 6 | Representação dos canais | Sub-linhas A/B/C nas etapas 1–2; marcador *(convergência)* nas etapas 3–4 |

---

## Fail Points Identificados

O blueprint registra 13 fail points distribuídos ao longo das 4 etapas. Os principais hipotéticos são:

| Tag | Descrição resumida |
| :--- | :--- |
| `[H_Interface_Celeste]` | Funil de exclusão digital na triagem via menu textual automático |
| `[H_Fila]` | Waiting Room do Zoom sem indicador de posição ou tempo estimado |
| `[H_Fantasma]` | Risco de abandono precoce do canal por ausência de feedback |
| `[H_Gargalo_WhatsApp]` | Ciclo de correções de documentos no WhatsApp podendo durar dias |
| `[H_Deslocamento_Contraditório]` | Cidadão precisa ir ao fórum para acessar serviço concebido como remoto |
| `[H_Autenticacao]` | Verificação de identidade via exibição de documento na webcam |
| `[H_Telas]` | Servidor operando PJe em tela paralela durante atendimento ao vivo |
