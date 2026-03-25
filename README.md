# 📊 Análise de dados:Identificando Causas de Cancelamento

Este projeto utiliza **Python** e a biblioteca **Pandas** para realizar uma análise de dados completa em uma base de clientes, buscando entender os motivos pelos quais os usuários cancelam seus serviços. Através da biblioteca **Plotly**, são gerados gráficos interativos que facilitam a extração de insights estratégicos.

---

##Tecnologias e Bibliotecas
* **Python 3.x**
* **Pandas**: Manipulação e tratamento de dados (Data Cleaning).
* **Plotly Express**: Criação de visualizações dinâmicas e histogramas.
* **NumPy & Openpyxl**: Suporte para operações matemáticas e leitura de arquivos.

---

## Passo a Passo do Projeto

### 1. Importação e Visualização
A base de dados é carregada via Pandas. Nesta etapa, o foco é entender a estrutura dos dados, tipos de colunas e identificar possíveis inconsistências.

### 2. Tratamento de Dados (Data Cleaning)
Para garantir uma análise precisa, foram aplicadas as seguintes etapas de limpeza:
* **Remoção de Colunas Inúteis**: Exclusão de IDs e informações que não agregam valor estatístico.
* **Tratamento de Valores Vazios (NaN)**: Utilização do método `dropna()` para remover registros incompletos.
* **Reset de Índices**: Reorganização da tabela após a limpeza das linhas.

### 3. Análise Inicial
Cálculo da taxa de cancelamento total para entender o tamanho do problema.
* Utilização de `value_counts()` para contar cancelamentos.
* Exibição de dados percentuais para visão macro do Churn.

### 4. Análise de Causa Raiz (Visualização)
Criação de um loop automatizado para gerar gráficos de todas as variáveis da tabela comparadas à coluna de cancelamento.
* **Ferramenta**: `px.histogram`.
* **Diferencial**: O uso do parâmetro `color="cancelou"` permite identificar padrões comportamentais de forma visual e imediata.

---

## Como Executar o Projeto

1. Certifique-se de ter o Python instalado.
2. Instale as dependências:
   ```bash
   pip install pandas plotly numpy openpyxl nbformat ipykernel
