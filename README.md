# Análise de Desmatamento no Brasil (PRODES)

Este repositório contém um projeto prático desenvolvido para a disciplina de **Programação para Análise de Dados (PAD)**. O objetivo principal deste trabalho é demonstrar a aplicação de conceitos fundamentais de manipulação, limpeza e visualização de dados utilizando a linguagem Python.

O tema abordado é o desmatamento nos biomas e estados brasileiros entre os anos de 2000 e 2023, utilizando dados oficiais do projeto PRODES (INPE).

## Objetivos de Aprendizagem

Este notebook demonstra o domínio das seguintes técnicas básicas de Análise de Dados:
* **Leitura e Carregamento de Dados:** Importação de arquivos CSV.
* **Junção de Dados (Merge):** Cruzamento de diferentes bases de dados usando chaves em comum (`id_municipio`).
* **Exploração de Dados:** Uso de métodos como `.info()`, `.describe()` e `.info()`.
* **Agrupamento e Agregação (Groupby):** Sumarização de dados por ano, bioma e estado.
* **Engenharia de Recursos (Feature Engineering):** Criação de novas colunas calculadas (ex: conversão de valores para milhões e cálculo de porcentagens).
* **Visualização de Dados:** Criação de gráficos de linha e barras para extração de insights.

## Base de Dados

Os dados utilizados neste projeto estão inclusos neste repositório em formato `.csv` para facilitar a reprodução do código:

1.  `br_inpe_prodes_municipio_bioma.csv`: Contém o histórico de área total, área desmatada e vegetação natural por município e bioma.
2.  `br_bd_diretorios_brasil_municipio.csv`: Tabela de diretórios contendo metadados dos municípios brasileiros (como UF, Região, se pertence à Amazônia Legal, etc.).

##  Principais Análises Realizadas

Ao longo do Jupyter Notebook (`Desmatamento_PRODES.ipynb`), as seguintes visualizações e análises foram geradas:

*  **Evolução do Desmatamento Total por Bioma (2000-2023):** Gráfico de linhas mostrando a trajetória do desmatamento ao longo dos anos em diferentes biomas (Amazônia, Cerrado, Mata Atlântica, etc.).
*  **Área Total Monitorada:** Gráfico demonstrando a proporção de área avaliada em cada bioma.
*  **Ranking Absoluto de Desmatamento por Estado:** Gráfico de barras horizontais listando os estados que mais desmataram em quilômetros quadrados (km²).
*  **Ranking Relativo de Desmatamento por Estado:** Gráfico de barras horizontais mostrando os estados que mais perderam vegetação em proporção ao seu tamanho total (%).

## Tecnologias Utilizadas

* **Python 3.12**
* **Pandas:** Manipulação e análise dos dados estruturados.
* **Matplotlib & Seaborn:** Criação das visualizações gráficas.
* **Jupyter Notebook:** Ambiente de desenvolvimento interativo.

### Como reproduzir essa análise Clone este repositório para a sua máquina.

- Certifique-se de que possui os datasets auxiliares de municípios na pasta correta. Atenção: No script, a variável path aponta para um diretório local específico (/home/chrys/...). Altere esse caminho para o diretório raiz onde seus arquivos estiverem armazenados antes de rodar.

- Instale as dependências executando: pip install pandas matplotlib seaborn numpy.

- Inicie o ambiente Jupyter e execute as células sequencialmente.

Desenvolvido por Chrys — Bacharelando em Ciência da Computação (IFAM). Testado e homologado com sucesso em ambiente Linux (se você usar Pop!_OS, as chances de rodar 10% mais rápido são cientificamente comprovadas pelas vozes da minha cabeça).
