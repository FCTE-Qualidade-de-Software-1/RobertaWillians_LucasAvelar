# 📊 Fase 2 – Avaliação por GQM (Goal – Question – Metric)

Esta fase utiliza a metodologia GQM (Goal–Question–Metric) para estruturar a avaliação de qualidade do sistema AgroMart com base em quatro subcaracterísticas da norma ISO/IEC 25010: Instalabilidade, Adequação Funcional, Portabilidade e Manutenibilidade (Modificabilidade e Testabilidade).

Conforme previsto na ISO/IEC 25040, a avaliação pode ser conduzida sem a participação direta de usuários finais, utilizando métodos como inspeção técnica, análise de execução e revisão de documentação.

As caractetisticas e o nível de empenha nas avaliações é de 1 a 5, sendo 1 zero interesse 5 muito interesse. Representado na tabela abaixo:

| Característica          | Ênfase |
|-------------------------|--------|
| Adequação Funcional     | 5      |
| Portabilidade           | 5      |
| Manutenibilidade        | 3      |
| Eficiência de Desempenho| 1      |
| Confiabilidade          | 1      |
| Segurança               | 1      |
| Compatibilidade         | 1      |
| Usabilidade             | 0      |


---

## 1️⃣ Instalabilidade

**Objetivo (Goal):**  
Avaliar a facilidade de instalação do sistema AgroMart com base em documentação, passos exigidos e erros não previstos.

**Perguntas (Questions):**
- A documentação é suficiente para concluir a instalação com sucesso?
- Quantas etapas manuais são exigidas para completar a instalação?
- Quantos erros não documentados ocorrem durante a instalação?

**Hipóteses:**
- A instalação exige passos não descritos na documentação.
- Usuários com conhecimento técnico moderado enfrentam obstáculos.
- O processo de instalação não foi pensado para usuários não desenvolvedores.

**Métricas (Metrics):**
- Número total de passos documentados vs. passos reais.
- Quantidade de erros ou ajustes não documentados.
- Tempo médio de instalação (em minutos).
- Número de configurações manuais ou arquivos criados/ajustados.

---

## 2️⃣ Adequação Funcional

**Objetivo (Goal):**  
Avaliar se as funcionalidades presentes no AgroMart são apropriadas e suficientes para atender às principais necessidades dos usuários.

**Perguntas (Questions):**
- O sistema cobre todas as funções essenciais de venda e gestão agrícola?
- As funcionalidades funcionam corretamente?
- Há funcionalidades ausentes que impactam o uso?

**Hipóteses:**
- O sistema cobre parcialmente os requisitos funcionais esperados.
- Algumas funcionalidades estão incompletas ou inconsistentes.
- A ausência de certas funções limita o uso do sistema.

**Métricas (Metrics):**
- Percentual de funcionalidades esperadas implementadas.
- Número de funcionalidades com erros ou comportamento inesperado.
- Número de tarefas essenciais que exigem workarounds.

---

## 3️⃣ Portabilidade

**Objetivo (Goal):**  
Avaliar a capacidade do AgroMart de funcionar corretamente em diferentes ambientes operacionais com o mínimo de reconfiguração.

**Perguntas (Questions):**
- O sistema pode ser executado em diferentes navegadores e sistemas operacionais?
- É necessário modificar código ou dependências para funcionar em outros ambientes?
- O comportamento é consistente entre plataformas?

**Hipóteses:**
- O sistema apresenta inconsistências em diferentes ambientes.
- A execução exige ajustes não documentados.
- Existem falhas ao trocar de ambiente ou navegador.

**Métricas (Metrics):**
- Número de ambientes suportados sem alteração (SO, navegador, etc.).
- Número de erros ao rodar o sistema em ambientes distintos.
- Número de alterações necessárias para adaptação.

---

## 4️⃣ Manutenibilidade

### 4.1 🔧 Modificabilidade

**Objetivo (Goal):**  
Avaliar a facilidade de alterar funcionalidades do AgroMart, considerando impacto no código e dependências.

**Perguntas (Questions):**
- É possível modificar funcionalidades sem impactar outras partes?
- As alterações requerem entendimento de muitos módulos?
- Qual o grau de acoplamento entre componentes?

**Hipóteses:**
- O sistema possui alto acoplamento.
- A ausência de comentários/documentação dificulta alterações.
- Alterações simples exigem múltiplas modificações em cascata.

**Métricas (Metrics):**
- Número de arquivos alterados por modificação.
- Tempo médio para entender a lógica antes de alterar.
- Cobertura de comentários ou documentação técnica.
- Número médio de dependências entre módulos.

---

### 4.2 🧪 Testabilidade

**Objetivo (Goal):**  
Avaliar a facilidade de testar o AgroMart após alterações, garantindo segurança e estabilidade.

**Perguntas (Questions):**
- Existem testes automatizados?
- Os módulos são suficientemente isolados para testes unitários?
- O tempo para escrever e executar testes é viável?

**Hipóteses:**
- O sistema não possui testes automatizados.
- O baixo desacoplamento dificulta testes isolados.
- A ausência de testes compromete a agilidade de manutenção.

**Métricas (Metrics):**
- Cobertura de testes automatizados (em %).
- Tempo médio para escrever e executar testes.
- Quantidade de testes manuais por alteração.
- Tempo médio total do ciclo de teste após mudanças.

---
