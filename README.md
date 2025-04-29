# challenge_AluraStore
# Análise de Vendas - Lojas AluraStoreBR

## 1. Propósito da Análise

Este projeto realiza uma análise exploratória dos dados de vendas de quatro fontes/lojas distintas, referidas como Loja 1 a Loja 4. O objetivo principal é consolidar os dados dessas lojas e extrair insights sobre:

* Padrões gerais de vendas.
* Desempenho de diferentes categorias de produtos e produtos específicos.
* Avaliação dos clientes 
* Comparação do faturamento entre as diferentes lojas/fontes de dados.

A análise visa fornecer uma compreensão abrangente do comportamento de compra dos clientes e do desempenho das vendas nas diferentes unidades ou fontes de dados.

## 2. Estrutura do Projeto

O repositório está organizado da seguinte forma:

* **/dados/** (Sugestão: Crie uma pasta para os dados)
    * `loja_1.csv`: Dados de vendas da Loja 1.
    * `loja_2.csv`: Dados de vendas da Loja 2.
    * `loja_3.csv`: Dados de vendas da Loja 3.
    * `loja_4.csv`: Dados de vendas da Loja 4.
* `AluraStoreBr.ipynb`: Notebook Jupyter contendo todo o processo de análise de dados, desde o carregamento, limpeza, tratamento, visualização e extração de insights.
* `README.md`: Este arquivo, contendo a descrição do projeto.
* `(Opcional) requirements.txt`: Arquivo listando as bibliotecas Python necessárias.

## 3. Exemplos de Gráficos e Insights Obtidos

O notebook `AluraStoreBr.ipynb` realiza diversas análises, gerando visualizações e insights como:

* **Visão Geral dos Dados:** Carregamento, tratamento inicial (tipos de dados, valores ausentes) e unificação dos dados das 4 lojas.
* **Vendas por Categoria:** Gráficos de barras mostrando as categorias de produtos mais vendidas em termos de quantidade e/ou valor total.
* **Avaliação Média:** Cálculo e visualização da avaliação média das compras
* **Produtos Mais/Menos Vendidos:** Listas e gráficos identificando os 3 produtos com maior e menor volume de vendas.

## 4. Instruções para Executar o Notebook

Para executar a análise contida no notebook `AluraStoreBr.ipynb`, siga os passos abaixo:

1.  **Clone o Repositório:**
    ```bash
    git clone https://github.com/dayanmoshe/challenge_AluraStore.git
    ```

2.  **Ambiente:**
    * Certifique-se de ter Python 3 instalado.
    * Recomenda-se o uso de um ambiente virtual (`venv` ou `conda`).

3.  **Instale as Dependências:**
    As principais bibliotecas utilizadas são Pandas para manipulação de dados e Matplotlib/Seaborn para visualização. Instale-as (ou use um arquivo `requirements.txt` se criar um):
    ```bash
    pip install pandas matplotlib seaborn jupyter notebook
    # ou pip install -r requirements.txt
    ```

4.  **Estrutura de Arquivos:**
    * Certifique-se de que os arquivos `loja_1.csv`, `loja_2.csv`, `loja_3.csv` e `loja_4.csv` estejam na mesma pasta que o notebook ou em uma subpasta (`/dados/`, por exemplo) e ajuste os caminhos de leitura no notebook se necessário.

5.  **Execute o Notebook:**
    * Inicie o Jupyter Notebook:
        ```bash
        jupyter notebook
        ```
    * Abra o arquivo `AluraStoreBr.ipynb` no seu navegador.
    * Execute as células sequencialmente (Shift + Enter).

    **Alternativa (Google Colab):**
    * Faça o upload do arquivo `AluraStoreBr.ipynb` para o Google Colab.
    * Faça o upload dos arquivos CSV para o seu Google Drive.
    * Adicione uma célula no início do notebook para montar seu Google Drive:
      ```python
      from google.colab import drive
      drive.mount('/content/drive')
      ```
    * Ajuste os caminhos de leitura dos arquivos CSV no notebook para apontar para a localização deles no seu Google Drive (ex: `'/content/drive/MyDrive/pasta_dados/loja_1.csv'`).
    * Execute as células sequencialmente.
