# 📘 Planejamento da Avaliação de Qualidade do AgroMart

##  Visão Geral do Planejamento

Este planejamento estabelece a estrutura e diretrizes do processo de avaliação de qualidade aplicado ao sistema **AgroMart**, com base na norma **ISO/IEC 25010** e na metodologia **GQM (Goal-Question-Metric)**. Conforme estabelecido na norma **ISO/IEC 25040**, a avaliação da qualidade de um sistema pode ser conduzida por avaliadores independentes, sem a necessidade da participação direta de usuários finais. Isso é possível por meio de métodos como **inspeção técnica, análise estática, testes estruturados e revisão de documentação**, desde que os critérios e métricas estejam previamente definidos de forma objetiva e reprodutível.


O plano está dividido em quatro fases principais:

1. Fase 1 – Escopo e Metas  
2. Fase 2 – Especificação por GQM e Características de Qualidade  
3. Fase 3 – Projeto da Avaliação  
4. Fase 4 – Execução e Coleta de Métricas
5. Gestão do projeto
6. Apresentação do projeto

---

## 🔹 Fase 1 – Escopo e Metas

Nesta fase, foi definido:

- **Software Avaliado:** AgroMart – uma plataforma de comercialização de produtos agroecológicos fundada no período da pandemia amparando a CSA (Comunidade que Sustenta a Agricultura) e usuários finais.
- **Objetivo Geral:** Avaliar e evidenciar a qualidade do AgroMart com foco em instalabilidade, adequação funcional, portabilidade e manutenibilidade.
- **Público-Alvo:** Usuários finais, equipe de desenvolvimento e comunidade de contribuidores open source.
- **Abordagem:** Inspeção técnica, testes manuais, testes automatizados e análise baseada em GQM.
- **ODS Relacionado:** Analisar em quais ODS da onu ele abrange e se encaixa.

---

## 🔹 Fase 2 – Especificação com GQM e ISO/IEC 25010

Nesta fase, foi aplicado o modelo GQM para estruturar a avaliação das seguintes subcaracterísticas da ISO/IEC 25010:

- **1️⃣ Instalabilidade**
- **2️⃣ Adequação Funcional**
- **3️⃣ Portabilidade**
- **4️⃣ Manutenibilidade** (Testabilidade)

Cada característica foi detalhada com:

- **Objetivo**
- **Perguntas**
- **Hipóteses**
- **Métricas**

> A estrutura completa da Fase 2 encontra-se na fase 2.

---

## 🔹 Fase 3 – Projeto da Avaliação

###  Atividades Planejadas

- Definição de **cenários de uso reais possíveis**
- Possível criação de **roteiros manuais** para instalação, cadastro, navegação e operação do sistema
- Estabelecimento de critérios de aceitação por cenário

###  Tipos de Testes

- **Testes manuais:** conduzidos pelo avaliador (Lucas Avelar) simulando usuários
- **Testes automatizados:** rodados em pipelines CI (Continuous Integration)
- **Análise de código e documentação:** para avaliar manutenibilidade

###  Instrumentos de Coleta

- Planilhas com tempos e erros
- Questionários de satisfação e feedback
- Logs de execução e relatórios do Lighthouse

###  Cronograma Sugerido

| Dia | Atividade |
|--------|-----------|
| 1 | Planejamento e definição dos cenários e critérios |
| 2 | Execução de testes automatizados |
| 2 | Sessões de testes manuais com coleta de dados |
| 3 | Análise, consolidação dos resultados e relatórios |

---

## 🔹 Fase 4 – Execução e Coleta de Métricas

### 📥 Execução dos testes

- Realizada pelo avaliador com base nos roteiros definidos
- Registro dos resultados e comparação com critérios definidos
- Uso de ferramentas como Lighthouse CI, cronômetro digital, formulários e planilhas

### 📊 Análise das Métricas

As métricas obtidas serão confrontadas com as hipóteses levantadas na Fase 2 para verificar:

- **Conformidade com os padrões ISO**
- **Forças e fraquezas do sistema**
- **Evidências para futuras melhorias**

---

## ✅ Resultados Esperados

- Diagnóstico da qualidade do AgroMart em quatro frentes técnicas
- Relatório estruturado para orientar melhorias futuras
- Referência metodológica para avaliações similares em software livre

---

