# Análise de Churn de Clientes - TelecomX

Este repositório contém a análise exploratória e o tratamento de dados do dataset de Churn de Clientes da TelecomX, culminando na geração de um relatório visual e uma tabela tratada para análise posterior.

## Estrutura do Repositório

*   `TelecomX_BR.ipynb`: Notebook Jupyter/Colab contendo todo o código Python para a extração, transformação e análise exploratória dos dados, incluindo a geração dos gráficos.
*   `TelecomX_BR_Tratada.xlsx`: Arquivo Excel contendo a tabela de dados original após o processo de transformação e limpeza, pronta para ser utilizada em outras ferramentas ou análises.
*   Imagens: Arquivos de imagem dos gráficos gerados no notebook, salvos para facilitar a incorporação em apresentações ou relatórios. (Ex: `grafico_cancelamento_genero.png`, `grafico_cancelamento_suporte.png`, etc.)

## Sobre o Projeto

O objetivo principal deste projeto é entender os fatores que levam os clientes da TelecomX a cancelar seus serviços (Churn). Através da análise de diferentes atributos dos clientes, como informações demográficas, serviços contratados e histórico de contrato, buscamos identificar padrões e insights que possam auxiliar a empresa a reduzir a taxa de churn.

## Análise Realizada (`TelecomX_BR.ipynb`)

O notebook `TelecomX_BR.ipynb` documenta as seguintes etapas:

1.  **Extração:** Leitura dos dados brutos a partir de uma URL em formato JSON.
2.  **Transformação:**
    *   Desaninhamento de colunas complexas (como 'customer', 'phone', 'internet', 'account' e 'account_charges').
    *   Renomeação das colunas para português para maior clareza.
    *   Tratamento da coluna 'Churn', convertendo-a para um formato booleano.
    *   Criação de novas features, como a `contas_diarias` e `quantidade_servicos`.
3.  **Carga e Análise Exploratória:**
    *   Análise descritiva das colunas numéricas e categóricas.
    *   Visualização da distribuição de cancelamentos por gênero.
    *   Análise da relação entre cancelamento e o serviço de suporte técnico.
    *   Exploração da distribuição de cancelamentos pelo tempo de contrato, categorizado em faixas de meses/anos.
    *   Investigação da taxa de cancelamento em função da quantidade de serviços contratados.
    *   Análise combinada da taxa de cancelamento, suporte técnico e quantidade de serviços para um subset específico de clientes.
    *   Geração dos gráficos correspondentes a cada análise, salvos como arquivos PNG.

## Dados Tratados (`TelecomX_BR_Tratada.xlsx`)

O arquivo `TelecomX_BR_Tratada.xlsx` é o resultado direto da etapa de transformação. Ele contém o dataset com as colunas desaninhadas, renomeadas, e as novas features criadas. Este arquivo é útil para quem deseja utilizar os dados tratados em outras ferramentas (como Power BI, Tableau) ou realizar análises adicionais sem a necessidade de rodar o código de tratamento novamente.

## Como Utilizar

### Executando o Notebook no Google Colab

1.  Abra o Google Colab (colab.research.google.com).
2.  Vá em "Arquivo" -> "Fazer upload de notebook".
3.  Selecione o arquivo `TelecomX_BR.ipynb` do seu computador.
4.  Execute as células sequencialmente (Ctrl + Enter em cada célula ou "Ambiente de execução" -> "Executar tudo"). O notebook baixará o dataset original, realizará o tratamento, gerará os gráficos e salvará o arquivo Excel e as imagens no ambiente do Colab.
5.  Para baixar o arquivo Excel e os gráficos, você pode usar o ícone de pasta no lado esquerdo do Colab e fazer o download dos arquivos gerados (`analise_telecom_tratada.xlsx` e os arquivos `.png`).

### Visualizando o Arquivo Excel

Abra o arquivo `TelecomX_BR_Tratada.xlsx` em qualquer software de planilha (Microsoft Excel, Google Sheets, LibreOffice Calc, etc.) para explorar os dados tratados.

Atenciosamente,

[Ulisses de Pinho Rodrigues Neto]
