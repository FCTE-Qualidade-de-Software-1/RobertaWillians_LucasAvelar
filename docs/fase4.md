##  **Objetivo da Execução**

Executar a avaliação da qualidade do sistema AgroMart de forma sistemática e rastreável, com base nas métricas definidas na Fase 2 (GQM). Esta etapa visa transformar os objetivos e hipóteses formuladas em observações concretas, coletadas por meio de testes, análises e inspeções. O propósito é obter evidências quantitativas e qualitativas que apoiem decisões sobre a evolução do software, mesmo sem a participação de usuários finais, conforme permitido pela ISO/IEC 25040.

##  **Método de Avaliação**

A avaliação será conduzida por meio de testes direcionados, inspeções técnicas e observações internas da equipe avaliadora. As métricas especificadas no modelo GQM serão aplicadas sobre os seguintes tipos de atividades:

- Testes manuais em ambiente controlado (navegação, cadastro, compra, etc.).
- Análise de código e documentação.
- Execução de scripts automatizados (quando aplicável).
- Inspeção de comportamento em diferentes ambientes e navegadores.

Serão utilizados tanto métodos **quantitativos** (tempo, número de erros, etapas de instalação) quanto **qualitativos** (percepção de clareza, fluidez e robustez do sistema).

## 1️ **Instalabilidade**

###  **Método de Avaliação**  
A avaliação foi realizada a partir da tentativa de instalação completa do sistema AgroMart, seguindo exclusivamente as instruções fornecidas na documentação disponível no repositório. O processo incluiu a instalação tanto do back-end (Strapi) quanto do front-end (aplicativo mobile via ExpoGo). Foram analisados o número de etapas necessárias, a existência de erros não previstos, o tempo total de instalação e os ajustes manuais exigidos.

---

###  **Resultados Observados**

**Back-end (Strapi):**

- **M1**: Documentação indicava 6 passos; na prática, foram necessários 8 passos, incluindo a criação de arquivos e ajustes não previstos.

- **M2**: Foram encontrados ao menos 2 erros não documentados, exigindo soluções manuais.

- **M3**: O tempo total para concluir a instalação foi de aproximadamente 100 a 120 minutos.

- **M4**: Foram necessárias modificações em dois arquivos – criação de um novo e ajuste em outro.

**Front-end (Aplicativo):**

- **M1**: Documentação indicava 4 passos; na prática, foram necessários 7 passos, incluindo a instalação do app ExpoGo e substituição da versão por um APK disponível so em Android.

- **M2**: Foram encontrados 2 ajustes não documentados: (1) necessidade de instalar o ExpoGo manualmente e (2) necessidade de alterar a versão do app.

- **M3**: Tempo médio de instalação foi de aproximadamente 20 minutos.

- **M4**: Nenhuma modificação manual ou criação de arquivo foi necessária.

---

###  **Interpretação dos Resultados**

- **H1** (A instalação pode ser concluída com base exclusivamente na documentação disponível): ❌ Refutada. A documentação não cobre todos os passos reais, exigindo ações fora do previsto.

- **H2** (Usuários com conhecimento técnico moderado conseguem instalar o sistema sem grandes dificuldades): ⚠️ Parcialmente refutada. Mesmo com conhecimento técnico, a instalação exigiu ações mais complexas e demoradas que o previsto.

- **H3** (O processo de instalação foi projetado de forma acessível, mesmo para quem não é desenvolvedor): ❌ Refutada. A instalação depende de conhecimento técnico e ajustes não triviais.

---

###  **Conclusão**

O processo de instalação do sistema AgroMart apresenta fragilidades significativas na documentação e suporte ao usuário. A ausência de instruções completas e a necessidade de soluções improvisadas comprometem a **Instalabilidade**, especialmente para perfis não desenvolvedores. O tempo excessivo para instalação, aliado à ausência de informações sobre requisitos críticos como ExpoGo e APKs personalizados, reforça a necessidade de revisão do material de suporte e simplificação do processo.



##  **2 Execução da Avaliação – Adequação Funcional**

###  **Objetivo**
Avaliar se as funcionalidades presentes no AgroMart são apropriadas e suficientes para atender às principais necessidades dos usuários e desenvolvedores.

---

### **M1 – Percentual de funcionalidades esperadas implementadas**

Foram definidos **10 requisitos funcionais essenciais** com base no escopo do AgroMart serão esses: criar conta, cadstro de enderço, comprar cestas, relatórios, login e boões home, busca, meus dados, sair, adicionar.

- Funcionalidades totalmente implementadas: **8**

- Funcionalidades parcialmente implementadas: **2**

- Funcionalidades ausentes: **0**

tabela dos resultados:

| Funcionalidade           | Status                   |
|--------------------------|--------------------------|
| Criar Conta              | ❌  Funciona parcialmente|
| Cadastro de Endereço     | ❌ Não Funciona          |
| Comprar Cestas           | ✅ Funciona              |
| Cadastrar CSA            | ❌ Não Funciona          |
| Login                    | ✅ Funciona              |
| Botão Home               | ✅ Funciona              |
| Botão Busca              | ✅ Funciona              |
| Botão Meus Dados         | ✅ Funciona              |
| Botão Sair               | ✅ Funciona              |
| Botão Adicionar          | ✅ Funciona              |

**Resultado Final:** 70% das funcionalidades estão totalmente implementadas.  
💡 *A hipótese H1 (sistema cobre os principais requisitos) é **parcialmente confirmada***.

---

###  **M2 – Número de funcionalidades com erros ou comportamento inesperado**

Durante a avaliação prática, foram identificados os seguintes problemas:

- O fluxo de venda não atualiza corretamente o estoque.

- A edição de produto falha quando há campos vazios.

- Em alguns testes, o login não redireciona corretamente.

**Total de falhas identificadas:** **3 funcionalidades** com comportamento inesperado.  
💡 *A hipótese H2 (funcionalidades operam de forma consistente) é **refutada***.

---

###  **M3 – Número de tarefas essenciais que exigem *workarounds***

Durante o uso, foram necessários contornos (workarounds) nas seguintes situações:

- Avaliador teve que reabrir a aplicação após login mal-sucedido.

- Algumas edições só funcionavam se todos os campos fossem preenchidos, mesmo os não obrigatórios.

**Total de tarefas com workarounds:** **3**  
💡 *A hipótese H3 (uso fluido da aplicação) é **refutada***.

---

###  **Conclusão**

A execução mostra que o AgroMart **possui boa base funcional**, mas ainda apresenta:

- Funcionalidades ausentes ou incompletas.

- Erros em operações fundamentais.

- Necessidade de ações manuais para contornar falhas.

Com base nisso, recomenda-se priorizar a **correção dos erros identificados** e a **finalização das funcionalidades pendentes** antes de uma entrega oficial do produto.

##  **3️ Portabilidade**

###  **Objetivo**  
Avaliar a capacidade do AgroMart de funcionar corretamente em diferentes ambientes operacionais com o mínimo de reconfiguração.

---

###  **Questões Investigadas**  

- O sistema pode ser executado em diferentes navegadores e sistemas operacionais?  

- É necessário modificar código ou dependências para funcionar em outros ambientes?  

- O comportamento é consistente entre plataformas?

---

###  **Hipóteses Avaliadas**  
**H1**: O sistema mantém comportamento consistente em diferentes ambientes operacionais e navegadores.  

**H2**: A execução do sistema ocorre sem a necessidade de ajustes não documentados.  

**H3**: O sistema opera corretamente em múltiplas plataformas sem falhas relevantes.  

---

###  **Métricas e Resultados**

**M1**: *Número de ambientes suportados sem necessidade de alteração (SO, navegador, etc.)*  

| Ambiente                       | Funcionalidade | Ajustes Necessários |
|-------------------------------|----------------|----------------------|
| Windows + Google Chrome       | ✅ Sim         | ❌ Não               |
| Windows + Microsoft Edge      | ✅ Sim         | ❌ Não               |
| Linux + Mozilla Firefox       | ✅ Sim         | ❌ Não               |
| Android + ExpoGo (Front-End)  | ⚠️ Parcial     | ✅ Sim               |

- **Resultado M1:** **3 de 4 ambientes funcionaram sem alterações** (75%).

**M2**: *Número de erros identificados ao rodar o sistema em diferentes ambientes*  
- Erros observados:  
  
  - O aplicativo que deveria estar na Play Store não estava mais disponível.  
  
  - Foi necessário baixar manualmente o **ExpoGo** e instalar um APK manualmente.  

- **Resultado M2:** **2 erros não previstos documentados**.

**M3**: *Número de modificações necessárias para adaptar o sistema a novos ambientes*  
- Foram necessárias:  

  - Instalação manual do APK da versão correta  

  - Mudança manual da versão no aplicativo para acessar o sistema  

- **Resultado M3:** **2 ajustes manuais foram exigidos.**

---

###  **Conclusão da Avaliação – Portabilidade**  

Apesar de funcionar corretamente em navegadores convencionais de desktop (Windows/Linux), o sistema apresentou **limitações significativas na portabilidade mobile**, exigindo intervenções manuais para o uso do front-end via aplicativo. As hipóteses **H1** e **H3** são **parcialmente confirmadas**, enquanto a **H2** é **refutada**, já que ajustes não documentados foram obrigatórios.

> 💡 Sugere-se que a documentação seja atualizada e que seja disponibilizado novamente o aplicativo na Play Store, ou que o processo de instalação por APK seja automatizado/documentado.

##  **4 Testabilidade**

Nesta etapa, executamos a avaliação da subcaracterística **Testabilidade**, com base nas perguntas, hipóteses e métricas definidas na Fase 2, conforme a abordagem GQM.

---

###  **Objetivo**
Avaliar a facilidade de testar o AgroMart após alterações, garantindo  estabilidade.

---

###  **Questões Respondidas**

**Q1: Existem testes automatizados?**  
 Sim. O sistema possui uma suíte de testes automatizados implementada com **Jest**, cobrindo os principais fluxos funcionais do AgroMart, como cadastro, autenticação e listagem de produtos.

**Q2: Os módulos são suficientemente isolados para testes unitários?**  
⚠️ Em sua maioria, sim. Embora a estrutura do projeto favoreça a separação de responsabilidades, foram encontrados **blocos de código duplicados e alta complexidade cognitiva** em algumas funções, o que indica oportunidades de melhoria no isolamento dos módulos.

**Q3: O tempo para escrever e executar testes é viável?**  
 Sim. O tempo médio de execução por arquivo de teste foi inferior a **200ms**, e a execução completa da suíte de testes ocorre em menos de **7 segundos**, permitindo iterações rápidas e frequentes durante o ciclo de desenvolvimento.

---

### ** Hipóteses Validadas**

**H1: O sistema possui testes automatizados que cobrem os principais fluxos de uso.**  
 Confirmada. A cobertura de testes automatizados está superior A **80%**, abrangendo rotas principais e comportamentos críticos.

**H2: Os módulos estão suficientemente desacoplados, permitindo testes unitários eficazes.**  
⚠️ Parcialmente confirmada. Apesar da estrutura modular, a presença de **código duplicado** e **complexidade elevada** em certas funções dificulta o isolamento ideal para testes unitários em alguns pontos.

**H3: O tempo necessário para testar alterações é adequado ao ciclo de desenvolvimento ágil.**  
 Confirmada. Os testes são executados de forma rápida e consistente, o que favorece ciclos ágeis e integração contínua.

---

###  **Métricas Coletadas**

| Código | Métrica                                             | Resultado     | Interpretação |
|--------|-----------------------------------------------------|---------------|----------------|
| M1     | Cobertura de testes automatizados (%)              | **88,9%**     | Excelente cobertura, garantindo confiança nos testes. |
| M2     | Tempo médio para escrever e executar testes         | ~**200ms** por arquivo | Rápido e adequado para ciclos ágeis. |
| M3     | Quantidade de testes manuais por alteração          | **0**         | A cobertura automatizada elimina a necessidade de testes manuais frequentes. |
| M4     | Tempo médio total do ciclo de teste após mudanças   | ~**7s**       | Compatível com integração contínua e validações recorrentes. |

---

###  **Conclusão**

A subcaracterística **Testabilidade** do sistema AgroMart apresenta **ótimo desempenho geral**, com indicadores positivos em cobertura, velocidade e consistência dos testes. Apesar de alguns pontos de atenção relacionados à complexidade do código e duplicações, o sistema demonstra estar bem preparado para ser testado com eficácia durante o seu ciclo de evolução.

** A testabilidade do sistema é considerada satisfatória, com potencial de evolução contínua.**

##  **Referências Bibliográficas**

- AGROMART – Documentação Oficial do Projeto  
  [https://agromart.github.io/docs/docs/intro](https://agromart.github.io/docs/docs/intro)

- ISO/IEC 25010 – Systems and Software Quality Requirements and Evaluation (SQuaRE)  
  [https://iso25000.com/index.php/en/iso-25000-standards/iso-25010](https://iso25000.com/index.php/en/iso-25000-standards/iso-25010)

- ISO/IEC 25040 – Evaluation process  
  [https://iso25000.com/index.php/en/iso-25000-standards/iso-25040](https://iso25000.com/index.php/en/iso-25000-standards/iso-25040)

- Repositório de Referência – Grupo Frances Allen (Turma 02, FCTE - UnB, 2025/1)  
  [https://fcte-qualidade-de-software-1.github.io/2025-1-T02-FRANCES-ALLEN/parte1/fase4/#cobertura-de-testes](https://fcte-qualidade-de-software-1.github.io/2025-1-T02-FRANCES-ALLEN/parte1/fase4/#cobertura-de-testes)

- ONU – Objetivos de Desenvolvimento Sustentável (ODS)  
  [https://brasil.un.org/pt-br/sdgs](https://brasil.un.org/pt-br/sdgs)
