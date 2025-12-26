# 📊 Análise de Evasão de Clientes — TelecomX

## 📌 Descrição do Projeto

Este projeto tem como objetivo analisar a **evasão de clientes (churn)** da empresa fictícia TelecomX, utilizando técnicas de **análise exploratória de dados (EDA)** com Python e Pandas.  
A evasão de clientes é um problema estratégico para empresas de telecomunicações, pois impacta diretamente a receita e a sustentabilidade do negócio.

A análise busca identificar **padrões, comportamentos e fatores associados ao cancelamento de serviços**, fornecendo insights que possam apoiar ações de retenção.

---

## 🎯 Objetivo da Análise

- Compreender o perfil dos clientes que evadem e dos que permanecem
- Identificar variáveis associadas à evasão (contrato, serviços, valores, etc.)
- Analisar a distribuição da evasão por variáveis categóricas e numéricas
- Explorar relações entre variáveis por meio de correlação (etapa opcional)

---

## 🗂️ Conjunto de Dados

Os dados foram obtidos a partir de uma **API no formato JSON**, contendo informações sobre:
- Perfil demográfico dos clientes
- Serviços contratados
- Informações de cobrança
- Status de evasão (churn)

Após o tratamento, o dataset final possui **7.267 registros** e **25 colunas**.

---

## 🧹 Limpeza e Tratamento de Dados

As principais etapas realizadas foram:

- Extração dos dados a partir da API (JSON)
- Normalização da estrutura do JSON em formato tabular
- Tratamento de valores ausentes
- Conversão de variáveis categóricas em valores binários quando necessário
- Padronização e tradução de nomes de colunas e categorias para português
- Criação de novas variáveis, como:
  - **Contas diárias** (valor mensal dividido por 30)
  - **Quantidade de serviços contratados**
- Criação de versões numéricas da variável de evasão para análises estatísticas

---

## 📈 Análise Exploratória de Dados (EDA)

Durante a análise exploratória, foram realizadas:

### 🔹 Análise da variável de evasão
- Distribuição de clientes que permaneceram vs. clientes que evadiram
- Visualização da proporção de churn

### 🔹 Evasão por variáveis categóricas
- Gênero
- Tipo de contrato
- Método de pagamento
- Tipo de serviço de internet
- Suporte técnico

Foram utilizados gráficos de barras (verticais e horizontais) para facilitar a comparação entre grupos.

### 🔹 Análise de variáveis numéricas
- Tempo de contrato
- Valor mensal dos serviços
- Total gasto pelo cliente
- Contas diárias

Comparações entre clientes que evadiram e os que não evadiram permitiram identificar padrões relevantes.

---

## 🔍 Análise de Correlação (Etapa Opcional)

Como etapa adicional, foi realizada a análise de correlação entre:
- Contas diárias e evasão
- Quantidade de serviços contratados e evasão
- Tempo de contrato e evasão

Essa análise ajuda a identificar variáveis com maior relação estatística com o churn e prepara o dataset para possíveis modelos preditivos.

---

## 💡 Principais Insights

- Clientes com **contrato mensal** apresentam maior taxa de evasão
- A ausência de **suporte técnico** está associada a maior churn
- Clientes com **menor tempo de contrato** tendem a evadir mais
- A **quantidade de serviços contratados** atua como fator de retenção
- Valores mais elevados de **contas diárias** mostram relação com a evasão

---

## 📌 Recomendações

Com base na análise, recomenda-se:

- Incentivar contratos de maior duração
- Oferecer suporte técnico como diferencial para retenção
- Criar estratégias específicas para clientes nos primeiros meses de contrato
- Avaliar políticas de preço e pacotes de serviços
- Utilizar os dados tratados como base para modelos preditivos de churn

---

## 🛠️ Tecnologias Utilizadas

- Python
- Pandas
- Matplotlib
- Google Colab

---

## 📁 Estrutura do Projeto

- `TelecomX_BR.ipynb` — Notebook principal com toda a análise
- `README.md` — Descrição do projeto

---

## ✍️ Observações Finais

Este projeto foi desenvolvido com foco em **clareza, organização e boas práticas em Data Science**, priorizando a interpretação dos dados e a geração de insights acionáveis.
