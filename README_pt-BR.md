# Análise de Faturamento - Online Retail

Este projeto tem como objetivo compreender o comportamento de vendas de uma base de e-commerce, identificando padrões de consumo, concentração de receita e nível de recorrência dos clientes.

A análise busca responder perguntas como:
- Qual fator tem maior impacto na geração de faturamento?
- Os clientes apresentam comportamento de recompra consistente (indicando fidelização)?
- Quais ações podem ser sugeridas para aumentar o faturamento?

---

## Fonte de Dados

Dataset público disponível em:
https://archive.ics.uci.edu/ml/machine-learning-databases/00352/Online%20Retail.xlsx

Contém informações transacionais como: Pedidos (InvoiceNo); Produtos (Description, StockCode); Quantidade e preço; Data da compra; Cliente (CustomerID); País

---

## Tratamento dos Dados

Antes da análise, foram realizados ajustes, como:

- Remoção de registros irrelevantes (taxas, frete, comissões, etc.)
- Criação da variável **Sales**
- Classificação de produtos por categoria (baseada em palavras-chave)
- Limpeza de inconsistências e valores ausentes

---

## Análises Realizadas

- Vendas ao longo do tempo  
- Distribuição de vendas por país  
- Faturamento por cliente  
- Produtos mais vendidos  
- Comportamento de recompra  
- Distribuição de faturamento (curva de Pareto) 
- Sinais de inatividade dos clientes 

---

## Principais Insights

- **Alta concentração geográfica**: ~85% do faturamento vem do Reino Unido  
- **Distribuição desigual de receita**: cerca de 30% dos clientes representam 80% do faturamento  
- **Recorrência relevante**: clientes com múltiplas compras concentram grande parte da receita  
- **Baixa dependência de produtos específicos**: vendas bem distribuídas entre produtos  
- **Comportamento de recompra heterogêneo**: não há padrão único de tempo entre compras  

---

## Limitações da Análise

- O tempo entre compras apresenta alta variabilidade, inviabilizando o uso de métricas simples como média
- A identificação de inatividade exige segmentação por perfil de cliente, não aplicada nesta etapa devido à limitação do histórico disponível  

---

## Dashboard

Um dashboard foi desenvolvido para visualização dos principais indicadores e padrões identificados.

---

## Conclusão

- A análise evidencia que o faturamento está fortemente associado a clientes recorrentes e concentrado em um país específico.  
- Há bom nível de recorrência: 65% dos clientes compraram mais de uma vez e 20% realizaram mais de 5 compras.
- Clientes de compra única representam apenas ~6% do faturamento, indicando concentração da receita em clientes recorrentes.

---

## Próximos Passos

- Segmentação de clientes por perfil de compra  
- Modelagem de churn/inatividade  
- Expansão da análise temporal  

---

## Arquivos
- Notebook Completo ipynb: A análise detalhada, incluindo tratamento dos dados, gráficos e construção dos insights, está disponível no notebook.
- Dashboard pbix: Desenvolvido para visualização dos principais indicadores e padrões identificados.

---

## Ferramentas e Conhecimentos Aplicados

- **Python (pandas, matplotlib)**  
- **ETL (Extract, Transform, Load)**   
- **Power BI**   
- **Análise Exploratória de Dados (EDA)** — identificação de padrões e comportamentos  
- **Análise de Negócio** — interpretação dos dados com foco em receita, recorrência e concentração  
- **Storytelling com Dados** — comunicação dos insights e limitações da análise  

