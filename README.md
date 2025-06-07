# Análise de Dados de Aluguel de Imóveis no Brasil

Este repositório contém notebooks Jupyter com uma análise completa de um conjunto de dados sobre aluguel de imóveis no Brasil, desde o pré-processamento e limpeza até a análise exploratória e visualização de dados.

## 📂 Visão Geral do Projeto

O objetivo deste projeto é realizar uma análise detalhada sobre dados de imóveis para alugar em diversas cidades brasileiras. O processo foi dividido em duas etapas principais, cada uma em seu próprio notebook:

1.  **Pré-processamento e Limpeza (`pre_processamento.ipynb`):** Preparação dos dados brutos para garantir a qualidade e a consistência das informações.
2.  **Análise Exploratória e Visualização (`analise_exploratoria.ipynb`):** Extração de insights através de gráficos e visualizações para entender as tendências e os padrões do mercado de aluguel.

## 📊 Conjunto de Dados

O dataset utilizado, `houses_to_rent_v2.csv`, contém informações sobre imóveis para alugar em cidades como São Paulo, Rio de Janeiro, Porto Alegre, Campinas e Belo Horizonte. Ele pode ser encontrado no Kaggle: [Brasilian Houses to Rent](https://www.kaggle.com/datasets/rubenssjr/brasilian-houses-to-rent/data).

Principais colunas:
- `city`, `area`, `rooms`, `bathroom`, `parking spaces`
- `floor`, `animal`, `furniture`
- `hoa (R$)`, `rent amount (R$)`, `property tax (R$)`, `fire insurance (R$)`, `total (R$)`

## 🚀 Notebooks

### 1. `pre_processamento.ipynb` - Pré-processamento de Dados

Este notebook realiza a limpeza e a transformação dos dados brutos. As principais tarefas executadas são:
- **Renomeação de colunas** para facilitar a manipulação.
- **Tratamento de valores ausentes** na coluna `floor`.
- **Codificação de variáveis categóricas** (`animal`, `furniture`) para formato numérico.
- **Exportação** do DataFrame limpo como `casas_limpo.csv`.

### 2. `analise_exploratoria.ipynb` - Análise e Visualização de Dados

Com os dados já limpos, este notebook explora as informações através de visualizações, buscando responder a perguntas como:
- Como os imóveis estão distribuídos entre as cidades?
- Qual a faixa de preço mais comum para os aluguéis?
- Como o número de quartos e banheiros influencia no valor do aluguel?
- Imóveis mobiliados são mais caros?
- A maioria dos proprietários aceita animais de estimação?

## 🛠️ Como usar

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/eznrr/houses_to_rent.git
    ```
2.  **Execute o notebook de pré-processamento:**
    - Abra e execute o `pre_processamento.ipynb` para gerar o arquivo `casas_limpo.csv`.
3.  **Execute o notebook de análise:**
    - Abra e execute o `analise_exploratoria.ipynb` para visualizar os gráficos e as análises.

## 📚 Bibliotecas Utilizadas
- **pandas:** Para manipulação e análise de dados.
- **numpy:** Para operações numéricas.
- **matplotlib & seaborn:** Para a criação de gráficos e visualizações.
- **re:** Para trabalhar com expressões regulares na limpeza de texto.