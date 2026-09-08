# 🎯 Projeto Prático: Gestão de Riscos Psicossociais e Ergonomia na Nova NR-1 (GRO/PGR)
## 📚 Caderno Temático Ativo de SST & Compliance Organizacional — Desafio Bootcamp DIO
Este repositório foi desenvolvido como entrega final para o Desafio de Projeto da **Digital Innovation One (DIO)**. O projeto demonstra a aplicação prática de inteligência artificial generativa — utilizando o **Gemini Notebook** (anteriormente conhecido como NotebookLM) — como uma ferramenta de **aprendizagem ativa e estruturação de conhecimento de alto nível** para a área de Saúde e Segurança do Trabalho (SST) e Recursos Humanos (RH).

O escopo do projeto consiste na tradução dos conceitos abstratos da **Nova NR-1 (Portaria MTE nº 1.419/2024)**, da **NR-17 (Ergonomia)** e de avaliações psicossociais (ARP) em uma esteira operacional viva de gestão, gerando ferramentas práticas de controle de riscos e auditoria para empresas, com foco no segmento de Mercado Atacadista.

---

## 🔍 1. Contexto e Objetivos

### Contexto de Negócio & Regulatório
A segurança e saúde no trabalho no Brasil vivenciam uma virada de paradigma. Com a vigência da nova redação do Capítulo 1.5 da NR-1, as empresas passam a ser obrigadas a incluir em seu **Gerenciamento de Riscos Ocupacionais (GRO)** e **Programa de Gerenciamento de Riscos (PGR)** os fatores de risco ergonômicos, incluindo especificamente os **riscos psicossociais** (estresse crônico, sobrecarga de trabalho, metas abusivas, liderança autocrática e assédio).

No mercado atacadista (*Cash & Carry*), este desafio é crítico devido à alta volumetria operacional, ritmos de trabalho intensos, equipes robustas de frentes de caixa e logística de expedição, além de um histórico desafiador de absenteísmo focado em adoecimentos osteomusculares (DORT/LER - CIDs Grupo M) e transtornos mentais/comportamentais (Ansiedade/Depressão - CIDs Grupo F).

### Objetivos do Caderno Temático
*   **Capacitação Ativa:** Demonstrar a utilização de IA generativa para co-criação de um sistema de gestão de SST que atenda rigorosamente aos requisitos legais da NR-1 e NR-17.
*   **Integração de SST & eSocial:** Construir e documentar o fluxo de informação entre o Inventário de Riscos (NR-1/PGR), os exames médicos (NR-7/PCMSO) e as obrigações acessórias do eSocial (Eventos S-2220 e S-2240).
*   **Operacionalização do PDCA:** Estruturar ferramentas de campo executáveis com prazos, responsáveis, planos de ação 5W2H e indicadores de eficácia focados na causa raiz organizacional.

---

## 📖 2. Curadoria de Fontes (Grounding)

Para garantir a blindagem regulatória do caderno temático e mitigar qualquer risco de "alucinação" da Inteligência Artificial, foram selecionadas **5 fontes abertas oficiais e científicas** para alimentar o Gemini Notebook:

1.  **Manual de Interpretação e Aplicação do Capítulo 1.5 da NR-1 — GRO (Portal Gov.br / MTE 2026):** Guia oficial emitido pela Secretaria de Inspeção do Trabalho (SIT) que uniformiza a interpretação dos conceitos de perigo, probabilidade, severidade e reavaliação de riscos.
2.  **Plano de Ação para Riscos Psicossociais NR-1: 7 Passos com Modelo Prático (Blog Taochi, 2026):** Metodologia prática para estruturar intervenções coletivas e organizacionais em 5W2H, destacando a necessidade de medidas focadas no trabalho real.
3.  **De Quanto em Quanto Tempo Refazer a Avaliação de Risco (Portal normar1, 2026):** Estudo prático sobre a dinâmica do ciclo de reavaliação e detalhamento das 6 situações que disparam a revisão imediata do PGR antes do prazo limite de 2 anos.
4.  **Como Integrar o eSocial com o GRO e o PGR (Portal NR1, 2026):** Artigo de engenharia de conformidade mostrando o mapeamento de riscos e exames sob a ótica dos eventos S-2220 e S-2240, alinhados à Tabela 24 do eSocial.
5.  **Programa de Gerenciamento de Riscos (Prefeitura Municipal de São José do Ouro/RS, 2022):** Documento real de PGR utilizado como benchmarking para modelagem de critérios qualitativos de probabilidade/severidade e cálculo do Indicador da Qualidade das Condições de Trabalho (IQCT).

---

## 🛠️ 3. Engenharia de Prompts & "Cicatrizes" (Troubleshooting)

Um dos pontos mais ricos desse projeto foi o processo colaborativo de co-criação. Documentar as perguntas e os desafios de interação (cicatrizes) demonstra a maturidade técnica em extrair o melhor de uma IA.

### 💬 Prompts Estratégicos Utilizados e Resultados Obtidos

#### **Prompt 1: Simulação por Cargo (Trabalho Real vs. Prescrito)**
> *“Vamos realizar uma simulação prática para o cargo de Operador de Caixa no ambiente de Mercado Atacadista. Calcule o NRO para dois riscos críticos (ergonômico físico e psicossocial) usando uma matriz 5x5 e estruture um plano de ação 5W2H focando na causa raiz organizacional.”*

*   **Resultado da IA:** A IA diferenciou com precisão o "trabalho real" da frente de caixa (manuseio de fardos pesados de 15kg a 30kg e pressão emocional pelo desconto de quebra de caixa) e calculou o Nível de Risco Ocupacional (NRO = 12, Risco Moderado).
*   **Plano Proposto:** Instalação de pistolas ópticas sem fio (engenharia) e revisão da política interna de quebra de caixa estabelecendo margens de tolerância (organizacional), rejeitando "palestras de prateleira" como controles primários.

#### **Prompt 2: Sincronização e Triangulação PCMSO-PGR**
> *“Como podemos integrar os dados médicos do PCMSO (atestados CIDs F e M) ao Inventário do PGR na prática, garantindo que o eSocial se mantenha atualizado sem criar processos redundantes?”*

*   **Resultado da IA:** A IA sugeriu um fluxo de triangulação epidemiológica em 5 passos (POP), disparando a reavaliação do PGR sempre que o médico do trabalho identificar adoecimento relacionado às atividades (gatilho d do item 1.5.4.4.6 da NR-1). Isso resulta em uma nova carga automatizada para o evento S-2240 e atualização do prontuário clínico (S-2220).

---

### 🩹 As "Cicatrizes" do Processo (Troubleshooting)

Durante o desenvolvimento do projeto prático, duas intercorrências críticas ocorreram no pipeline do **Content Studio** do Gemini Notebook, exigindo adaptabilidade técnica e engenharia de solução:

1.  **A Falha na Geração de Slides do Content Studio:**
    *   *O que aconteceu:* Ao tentar compilar a "Apresentação Executiva" para a Diretoria, a esteira externa de processamento de imagens e diagramas sofreu *timeouts* e quebras de compilação em segundo plano. Isso se deu pela complexidade das equações matemáticas e descrição exaustiva de múltiplos cargos enviadas no prompt original.
    *   *Como resolvemos (Troubleshooting):* Reduzi as restrições slide-a-slide e simplifiquei o prompt para um "Pitch Executivo Curto de 5 Slides" focado exclusivamente em métricas de alto impacto (ROI da prevenção, alíquota FAP, compliance digital com eSocial e cronograma de 6 fases). A simplificação reduziu o processamento do pipeline e a apresentação foi gerada com sucesso.
    *   *Alternativa Programática de Segurança:* Como plano de contingência para evitar falhas de renderização em nuvem, criei um script Python usando bibliotecas locais (fpdf2) no ambiente de computação seguro da IA para gerar de forma síncrona um roteiro detalhado de objeções em PDF (`roteiro-apresentacao-diretoria.pdf`), garantindo a entrega do material à diretoria mesmo diante de instabilidades externas.

2.  **A Estaticidade da Tabela de Prioridades:**
    *   *O que aconteceu:* A priorização de prazos padrão no Plano de Ação (ex: 3 meses para Risco Alto) ignorava o fator de escala humana.
    *   *Como resolvemos (Troubleshooting):* Foi introduzido um prompt de refino forçando a aplicação do **multiplicador de pessoas expostas** (ex: 45 ajudantes de carga expostos ao mesmo risco ergonômico). Isso permitiu otimizar o cronograma e diminuir o prazo de implementação de 90 para 30 dias de forma dinâmica na planilha Excel e no relatório em PDF.

---

## 📘 4. Miniguia de Estudo (Entrega Final)

### 📈 Resumos Estruturados do Assunto

#### **A. Trabalho Prescrito vs. Trabalho Real**
Uma gestão de riscos psicossociais eficiente deve desconsiderar descrições meramente burocráticas de cargo. O foco do diagnóstico é o **Trabalho Real** (o que o colaborador executa na prática para lidar com as variabilidades e pressões do dia a dia). A discrepância entre o que a empresa exige (metas) e as ferramentas que disponibiliza (infraestrutura) é a principal geradora de ansiedade, esgotamento e DORT.

#### **B. O Cálculo Dinâmico do NRO (Nível de Risco Ocupacional)**
O NRO é determinado pela fórmula regulamentar:
$$\text{NRO} = \text{Probabilidade (P)} \times \text{Severidade (S)}$$
A gradação da probabilidade é influenciada diretamente pelo cumprimento de requisitos legais (NRs) e pela eficácia real dos controles existentes. Se uma empresa não cumpre um requisito específico da NR-17 (como fornecer assentos reguláveis para operadores), a probabilidade deve ser classificada no nível máximo (5 - Muito Provável), até que a medida corretiva seja implementada e o risco residual seja reavaliado.

#### **C. Compliance Digital com o eSocial (Eventos SST)**
A conformidade trabalhista e previdenciária não é estática. A emissão de Atestados de Saúde Ocupacional (ASOs) deve refletir o inventário de riscos do PGR:
*   **Evento S-2220 (Monitoramento da Saúde):** Envia dados clínicos baseados no PCMSO (que por sua vez baseia-se nos riscos químicos, físicos, biológicos e ergonômicos mapeados no PGR).
*   **Evento S-2240 (Condições Ambientais/Agentes Nocivos):** Envia a carga de exposição e a eficácia real dos EPCs/EPIs definidos no Plano de Ação do PGR.

---

### 📝 Glossário de Conceitos Aprendidos

*   **GRO (Gerenciamento de Riscos Ocupacionais):** Processo contínuo e sistemático baseado no ciclo PDCA para identificar, avaliar, controlar e monitorar os riscos em todos os estabelecimentos da organização.
*   **PGR (Programa de Gerenciamento de Riscos):** A materialização do GRO em forma de programa documentado, composto obrigatoriamente por dois documentos base: o Inventário de Riscos e o Plano de Ação.
*   **ARP (Avaliação de Riscos Psicossociais):** Diagnóstico das condições organizacionais e das relações socioprofissionais de trabalho por meio de questionários científicos (ex: COPSOQ, HSE).
*   **AEP (Avaliação Ergonômica Preliminar):** Análise inicial e obrigatória de todas as situações de trabalho para identificação de perigos físicos e psicossociais decorrentes da atividade.
*   **AET (Análise Ergonômica do Trabalho):** Estudo ergonômico aprofundado e pontual, exigido por gatilhos específicos (como recomendação do PCMSO, ineficácia da AEP ou ocorrência de acidentes).
*   **NRO (Nível de Risco Ocupacional):** Índice resultante da combinação de probabilidade e severidade que define a prioridade de controle de cada risco.
*   **DET (Domicílio Eletrônico Trabalhista):** Plataforma digital federal de fiscalização e comunicação direta entre a Inspeção do Trabalho e o empregador, exigindo respostas e defesas rápidas.
*   **FAP (Fator Acidentário Previdenciário):** Multiplicador sobre a alíquota do RAT (de 0,5 a 2,0) que premia ou pune as empresas de acordo com seu histórico de afastamentos acidentários.

---

### 💻 Prompts Reutilizáveis para Revisão Técnica

#### **Prompt 1: Auditoria de Coerência de Plano de Ação (Evitar Planos de Prateleira)**
```markdown
Atue como um Auditor Fiscal do Trabalho (AFT). Analise a consistência entre o seguinte perigo identificado no meu Inventário de Riscos e a respectiva medida de controle proposta no meu Plano de Ação. Verifique se a medida foca na causa raiz organizacional e se respeita a hierarquia de controles da NR-1:
- Perigo Mapeado: [Inserir Perigo, ex: Ritmo intenso de trabalho e horas extras exaustivas na Expedição]
- Medida Proposta: [Inserir Medida, ex: Palestra sobre resiliência e treinamento de gestão de tempo]
Identifique inconformidades e proponha as correções ideais.

Prompt 2: Análise de Gatilhos para Gestão de Mudanças (PDCA)
Com base nas 6 situações de revisão imediata do PGR descritas na NR-1, avalie o seguinte cenário real que está acontecendo na minha empresa: [Descrever mudança, ex: Fusão de duas equipes do administrativo e corte de 25% do quadro de pessoal].
Indique:
1) Quais gatilhos da NR-1 foram ativados?
2) Quais áreas (RH, Gestão, SESMT) devem ser notificadas?
3) Quais documentos do PGR e eventos do eSocial precisam ser atualizados e em qual prazo?

Prompt 3: Modelagem de Medidas Organizacionais da Causa Raiz
Sou ergonomista e preciso propor medidas de prevenção para um setor que apresentou pontuação crítica (vermelha) na dimensão de "Justiça Organizacional" e "Demandas Cognitivas" no questionário COPSOQ II. 
Forneça uma lista de 5 medidas administrativas e organizacionais de custo baixo/moderado que atuem diretamente na organização do trabalho do setor de [Inserir Setor, ex: Faturamento Financeiro], contendo a justificativa técnica com base na NR-17 e o indicador de monitoramento para validar a eficácia.

🛠️ 5. Ecossistema de Artefatos Gerados no Gemini Notebook
Durante a execução desse estudo prático de compliance, foram desenvolvidos 10 artefatos funcionais para o projeto, organizados e disponíveis para consulta e exportação:

📁 Arquivos Operacionais e Técnicos:
planilha-gestao-riscos.xlsx: Planilha de gestão integrada contendo a matriz 5x5 automatizada e o plano de ação estruturado em 5W2H.

relatorio-implementacao-nr1.pdf: Manual técnico detalhando as diretrizes gerais de governança, o checklist de AEP e o modelo de comunicado de segurança psicológica.

relatorio-caixa-rh-atacado.pdf: Relatório técnico setorial específico para as funções de Operador de Caixa e profissionais de Recursos Humanos do segmento atacadista.

pop-integracao-pcmso-pgr.pdf: Procedimento Operacional Padrão de integração de fluxos e dados epidemiológicos entre a Medicina e a Segurança do Trabalho.

guia-bolso-lideres-perguntas.pdf: Um guia prático de bolso com as 10 perguntas de auditoria e inspeção visual para líderes em campo.

roteiro-apresentacao-diretoria.pdf: O roteiro estratégico de pitch e manual de tratamento de objeções financeiras, jurídicas e de eSocial para a diretoria.

🎥 Recursos Multimídia e Educacionais (Renderizados pelo Content Studio):
Apresentação Executiva GRO e Riscos Psicossociais [Slide Deck]: Apresentação de slides de alta performance para a alta liderança.

Guia de Execução do PGR: Liderança e Riscos Psicossociais [Vídeo]: Um explainer video animado explicando as 6 fases do cronograma.

Riscos psicossociais na NR-1 sem papelada [Áudio Overview]: Um podcast dinâmico de sensibilização e aculturamento das lideranças sobre a NR-1.

Mapa Mental das Fases do PGR/GRO (NR-1) & Cartões Didáticos [App]: Aplicativos dinâmicos de fixação rápida para responsáveis e membros do SESMT.

