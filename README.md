# Pipeline-de-Dados-com-Databricks-para-Analise-de-Vendas-em-E-commerce
Projeto de engenharia de dados com Databricks, que constrói um pipeline em camadas (bronze, silver e gold) para transformar dados de e-commerce em tabelas analíticas, permitindo consultas sobre vendas, produtos, cidades e uso de cupons.


## 🧠 Cenário

Uma empresa de e-commerce deseja entender melhor o perfil de seus clientes e acompanhar as vendas em tempo quase real. A área de marketing precisa explorar os dados para campanhas e promoções, enquanto os gestores querem monitorar as vendas.

## 🛠️ Solução

Foi desenvolvido um pipeline de dados utilizando Databricks e PySpark, com as seguintes etapas:

- **Bronze Layer**: ingestão dos dados brutos do arquivo `ecommerce.json`.
- **Silver Layer**: transformação dos dados, conversão de timestamps, explosão de arrays e limpeza.
- **Gold Layer**: criação de tabelas analíticas:
  - `cidades_gold`
  - `produtos_gold`
  - `vendas_gold`

## 📊 Consultas realizadas
1. Valor total de vendas com uso de cupom.
2. Ranking dos 5 produtos mais vendidos em junho/2020.
3. Cidades que aparecem em mais estados.
4. Pivot de vendas por item agrupado por cidade e estado.

## 📁 Arquivos

- `atividade-final.html`: versão interativa do notebook.
- `atividade-final.pdf`: versão em PDF do trabalho.
- `notebooks/pipeline_ecommerce.ipynb`: notebook com o pipeline (opcional).
- `sql/consultas.sql`: consultas SQL utilizadas.

## 🚀 Tecnologias

- Databricks
- PySpark
- SQL

📈 Insights do Projeto
Durante a construção do pipeline de dados, foi possível extrair diversos insights relevantes:

- Efetividade de Cupons: Identificação do valor total de vendas com uso de cupons, útil para avaliar campanhas promocionais.
- Produtos em Alta: Ranking dos produtos mais vendidos em junho/2020, com base na quantidade e valor total.
- Abrangência Geográfica: Cidades que aparecem em múltiplos estados, indicando maior presença nacional.
- Distribuição Regional de Vendas: Análise pivoteada por item vendido, agrupada por cidade e estado, revelando padrões regionais de consumo.
- Qualidade do Pipeline: Validação da arquitetura em camadas (bronze, silver, gold), garantindo integridade e eficiência na transformação dos dados.

 Autor
**Denilson Nunes do Lago** 
