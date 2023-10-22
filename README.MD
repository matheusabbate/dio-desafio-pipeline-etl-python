<div align="center">
  <img src="https://hermes.digitalinnovation.one/assets/diome/logo-full.svg" alt="Logo Bootcamp" width="80">
  <h1>Santander Bootcamp 2023 <br> Ciência de Dados com Python</h1>
  <img src="https://hermes.dio.me/tracks/03253ff0-95b9-4904-84e7-2063e9d6cb26.png" alt="Logo Bootcamp" width="220">
</div>

<h1 align="center">Contruindo um Pipeline ETL com Python - Analisando Dados de Fomento à Cultura</h1>

## Descrição do Projeto

Este projeto tem como objetivo analisar os projetos culturais apoiados pela Lei Rouanet, um programa de incentivo à cultura no Brasil. O foco está na coleta, transformação e análise de dados para aprimorar a transparência e a eficácia da Lei Rouanet. Serão apresentados dados sobre a captação de recursos segmentados por unidade federativa.

## Funcionalidades

- Coleta de dados relacionados a projetos culturais da Lei Rouanet.
- Limpeza e transformação de dados para análise.
- Criação de visualizações de dados.

## Etapas do Pipeline de ETL

### Extract

Nesta fase, os dados foram extraídos de um arquivo CSV. O código utiliza a biblioteca Pandas para ler os dados do arquivo CSV especificado no caminho 'seuarquivo.csv'. A função pd.read_csv é usada para carregar os dados do arquivo para um DataFrame do Pandas. Isso permite que os dados sejam manipulados e transformados nas próximas etapas do processo de ETL.

### Transform

Nesta fase, os dados foram transformados e organizados de acordo com as necessidades da análise. O principal objetivo foi reorganizar as colunas de 'Valor Captado' para que fiquem ao lado das colunas de anos correspondentes. Isso foi feito criando um novo DataFrame chamado df_com_anos. As colunas de 'Valor Captado' foram extraídas do DataFrame original e anexadas ao novo DataFrame com rótulos de ano correspondentes. Além disso, as colunas de 'Valor Captado' foram transformadas em valores numéricos, removendo vírgulas, pontos, espaços e a formatação 'R$'. Qualquer valor ausente foi preenchido com 0.

### Load

A fase de Load consiste em exibir os resultados e realizar qualquer ação adicional necessária, como calcular médias, criar gráficos ou até mesmo salvar os resultados transformados em um novo arquivo. Neste código, após a transformação, os resultados foram exibidos na forma do DataFrame df_com_anos com as tags de ano. Em seguida, o código calculou a média por região com base nos dados transformados e exibiu as médias por região no DataFrame media_por_regiao. Isso representa a fase de "Load" onde os resultados da transformação são apresentados para análise ou qualquer ação posterior.

## Instalação

1. Clone o repositório: `git clone https://github.com/matheusabbate/dio-desafio-pipeline-etl-python`
2. Acesse o diretório do projeto: `cd analise-lei-rouanet`
3. Instale as dependências: `pip install -r requirements.txt`

## 🧰 Ferramentas utilizadas

![PYTHON](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)
![GIT](https://img.shields.io/badge/Git-F05032.svg?style=for-the-badge&logo=Git&logoColor=white)
![GOOGLE COLAB](https://img.shields.io/badge/Google%20Colab-F9AB00.svg?style=for-the-badge&logo=Google-Colab&logoColor=white)
![VSCODE](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC.svg?style=for-the-badge&logo=Visual-Studio-Code&logoColor=white)

## Licença

Este projeto é distribuído sob a Licença [MIT](https://opensource.org/licenses/MIT).

## Contato

- Matheus Abbate dos Santos - santos.abbate@gmail.com
- Link para o projeto: [https://github.com/matheusabbate/dio-desafio-pipeline-etl-python](https://github.com/matheusabbate/dio-desafio-pipeline-etl-python)
