# Mini-Projeto DataView: Exploração e Análise de Dados de Vendas

## Sobre o projeto
O DataView PY é um projeto de análise exploratória de dados (EDA) de vendas, desenvolvido em Python usando o Google Colab. O notebook lê, limpa, transforma, analisa e visualiza um dataset sintético de vendas, gerando métricas e insights úteis para tomada de decisão. A base oficial escolhida para a análise final foi a **V2** (sem outliers).

## O que o projeto analisa
* Receita total e volume de vendas por mês e trimestre.
* Top produtos e categorias por receita.
* Desempenho e ticket médio por região.
* Segmentação de clientes por nível de gasto (Bronze, Prata, Ouro).
* Comparação entre os dados com e sem tratamento de outliers (v1 e v2).
* Exportação de relatórios consolidados em CSV e JSON.

## Conceitos Praticados
* **Lógica de programação:** Python, variáveis, condicionais (if/else) e tipos de dados.
* **Organização de Código:** Funções com parâmetros, retorno explícito e funções lambda.
* **Funções de Ordem Superior:** Implementação de callbacks para transformações.
* **Engenharia e Limpeza de Dados:** Tratamento de nulos, datas inválidas, strings com RegEx (`re`) e manipulação de datas (`datetime`).
* **Pandas:** DataFrames, `groupby`, filtros, e transformações.
* **NumPy:** Arrays, operações vetorizadas, broadcasting e transformação condicional com `np.select`.
* **Estatística:** Detecção e tratamento de outliers (método IQR).
* **Visualização:** Matplotlib e Seaborn para geração e exportação de gráficos (Linha, Barras e Boxplot).

## Como executar

### No Google Colab (Recomendado)
1. Clone este repositório ou faça o download da pasta.
2. Faça o upload da pasta do projeto para o seu Google Drive.
3. Abra o notebook `notebooks/dataview.ipynb` no Google Colab.
4. Execute a primeira célula para montar o Drive (`drive.mount`) e ajuste o caminho da variável `CAMINHO_PROJETO`.
5. Execute as células sequencialmente.

### Localmente (VS Code)
1. Instale o Python 3.10+ e o VS Code.
2. Instale as dependências executando: `pip install pandas numpy matplotlib seaborn`
3. Altere a variável `CAMINHO_PROJETO` no código para o caminho da sua pasta local.
4. Execute o script.

## Estrutura do projeto

DataView-Vendas/
├── data/
│   ├── raw/
│   │   └── vendas.csv
│   ├── processed/
│   │   ├── v1_com_outliers/
│   │   │   └── vendas_v1.csv
│   │   └── v2_outliers_tratado/
│   │       └── vendas_v2.csv
│   └── final/
│       └── vendas_final.csv
├── outputs/
│   ├── estatisticas_gerais.json
│   ├── metricas_por_mes.csv
│   ├── segmentacao_clientes.csv
│   └── graficos/
│       ├── dist_regiao.png
│       ├── receita_por_mes.png
│       └── top_produtos.png
├── README.md/
│
└── dataview.ipynb
