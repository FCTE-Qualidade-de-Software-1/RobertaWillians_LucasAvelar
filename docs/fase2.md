#  Fase 2 – Avaliação por GQM (Goal – Question – Metric)

Esta fase utiliza a metodologia GQM (Goal–Question–Metric) para estruturar a avaliação de qualidade do sistema AgroMart com base em quatro subcaracterísticas da norma ISO/IEC 25010: Instalabilidade, Adequação Funcional, Portabilidade e Manutenibilidade (Modificabilidade e Testabilidade).

Conforme previsto na ISO/IEC 25040, a avaliação pode ser conduzida sem a participação direta de usuários finais, utilizando métodos como inspeção técnica, análise de execução e revisão de documentação.

---

## 1️ Instalabilidade

###  Objetivo (Goal)
Avaliar a facilidade de instalação do sistema AgroMart com base em documentação, passos exigidos e erros não previstos.

---

###  Perguntas (Questions)
- A documentação é suficiente para concluir a instalação com sucesso? 
   
- Quantas etapas manuais são exigidas para completar a instalação?  

- Quantos erros não documentados ocorrem durante a instalação?  

---

###  Hipóteses  
**H1**: A instalação pode ser concluída com base exclusivamente na documentação disponível.  

**H2**: Usuários com conhecimento técnico moderado conseguem instalar o sistema sem grandes dificuldades.  

**H3**: O processo de instalação foi projetado de forma acessível, mesmo para quem não é desenvolvedor.  

---

###  Métricas (Metrics)  
**M1**: Número total de passos documentados vs. passos reais.  

**M2**: Quantidade de erros ou ajustes não documentados.  

**M3**: Tempo médio de instalação (em minutos).  

**M4**: Número de configurações manuais ou arquivos criados/ajustados.  

---

## 2️ Adequação Funcional

###  Objetivo (Goal)
Avaliar se as funcionalidades presentes no AgroMart são apropriadas e suficientes para atender às principais necessidades dos usuários.

---

###  Perguntas (Questions)
- O sistema cobre todas as funções essenciais de venda e gestão agrícola?  

- As funcionalidades funcionam corretamente?  

- Há funcionalidades ausentes que impactam o uso?  

---

###  Hipóteses  
**H1**: O sistema cobre os principais requisitos funcionais dos usuários.  

**H2**: As funcionalidades implementadas estão completas e operam de forma consistente.  

**H3**: As funções essenciais estão presentes e permitem o uso fluido da aplicação.  

---

###  Métricas (Metrics)  
**M1**: Percentual de funcionalidades esperadas implementadas.  

**M2**: Número de funcionalidades com erros ou comportamento inesperado.  

**M3**: Número de tarefas essenciais que exigem *workarounds*.  

---

## 3️ Portabilidade

###  Objetivo (Goal)  
Avaliar a capacidade do AgroMart de funcionar corretamente em diferentes ambientes operacionais com o mínimo de reconfiguração.  

---

###  Perguntas (Questions)  
- O sistema pode ser executado em diferentes navegadores e sistemas operacionais?  

- É necessário modificar código ou dependências para funcionar em outros ambientes?  

  

---

###  Hipóteses  
**H1**: O sistema mantém comportamento consistente em diferentes ambientes operacionais e navegadores.  

**H2**: A execução do sistema ocorre sem a necessidade de ajustes não documentados.  

**H3**: O sistema opera corretamente em múltiplas plataformas sem falhas relevantes.  

---

###  Métricas (Metrics)  
**M1**: Número de ambientes suportados sem necessidade de alteração (sistemas operacionais, navegadores, etc.).  

**M2**: Número de erros identificados ao rodar o sistema em diferentes ambientes.  

**M3**: Número de modificações necessárias para adaptar o sistema a novos ambientes.  

---

## 4️ Manutenibilidade 
Aqui o foco foi em uma subcaracterística de Manutenilidade, **Testabilidade**

### 4.1  Testabilidade

###  Objetivo (Goal)  
Avaliar a facilidade de testar o AgroMart após alterações, garantindo segurança e estabilidade.

---

###  Perguntas (Questions)  
- Existem testes automatizados?  

- Os módulos são suficientemente isolados para testes unitários?  

- O tempo para escrever e executar testes é viável?  

---

###  Hipóteses  
**H1**: O sistema possui testes automatizados que cobrem os principais fluxos de uso.  

**H2**: Os módulos estão suficientemente desacoplados, permitindo testes unitários eficazes.  

**H3**: O tempo necessário para testar alterações é adequado ao ciclo de desenvolvimento ágil.  

---

###  Métricas (Metrics)  
**M1**: Cobertura de testes automatizados (em %).  

**M2**: Tempo médio para escrever e executar testes.  

**M3**: Quantidade de testes manuais por alteração.  

**M4**: Tempo médio total do ciclo de teste após mudanças.  
