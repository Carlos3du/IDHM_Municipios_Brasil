# IDHM dos Municípios Brasileiros

Para melhor visualização da análise e seus resultados, entre no Colab utilizado para a análise:
https://colab.research.google.com/drive/1j5E7GUVw5dk78EgN-KH9pb4H3HBddcgP?usp=

<br>

## Cenário
Um gestor público solicitou a uma consultoria um levantamento de diversas informações sobre os municípios brasileiros. O objetivo é estudar características e propor políticas adequadas nas áreas de Educação, Saúde e aumento de Renda, e com isso responder algumas perguntas.

## Analise dos IDHM's

O primeiro indicador a ser analisado foi o Índice de Desenvolvimento Humano Municipal (IDHM), que é composto por três dimensões: longevidade, educação e renda. O índice varia de 0 a 1, sendo que quanto mais próximo de 1, maior o desenvolvimento humano.
Antes das análises que contemplam todos os municípios, foi feito um agrupamento desses municípios em Regiões (Norte, Nordeste, Centro-Oeste, Sul e Sudeste) para um melhor estudo geral e comparação entre diferentes regiões e estados.

De início, foi-se analisado o valor que separa os 25% dos municípios com os menores IDHM. E a partir desses resultados, agrupamos esses municípios com base nos seus estados e analisou-se a existencia de uma uma concentração em algum deles. Para demonstrar os resultados, foi feito um gráfico desses estados para visualisar melhor esses valores e suas porcentagens acumuladas em torno da linha de pareto.
Com base na classificação do IDHM determinada pela ONU:

<code>Baixo: < 0,550 | Médio: 0,550 - 0,699 | Alto: 0,700 - 0,799 | Muito Alto: >= 0,800</code>

Antes de tudo, foi feito a classificação dos IDHMs dos municípios baseados nessas 4 faixas.<br>
Foi feita uma análise nacional de cada região que entorne isso, como:
- A média dos tipos de IDHM (Geral, Renda e Educação) por região
- Classificação do IDHM (Baixo, Médio, Alto, ou Muito Alto) por região
- Comparação entre as médias dos IDHMs de educação e as médias das quantidades de empresas educacionais
- Analise geral dos dados de cada região (IDHM, IDHM  de Renda, IDHM Educacional e Renda per Capta

## Análise da Educação Nacional

Em primeiro plano, analisou-se as semelhanças e diferenças regionais entre as dispersões das quantidades de crianças de 1 a 4 anos. Dando continuidade, foi-se identificado os municípios que estão acima do 3º quartil nacional em relação à quantidade de crianças com idade entre 1 e 4 anos na região com a menor média de IDHM_Educacao (Nordeste). Esses resultados foram divididos por estado e para cada um deles foi feito um gráfico de barra para observar melhor os municípios individualmente

Em segundo plano, foi feita a identificação dos municípios que estão no 1º quartil nacional em relação à quantidade de empresas do setor educacional, destacando e priorizando os municípios com poucas empresas de educação. As analises feitas a seguir circundam essa seleção dos municípios descrita anteriormente:
- Comparação dos municípios com poucas empresas educacionais e seus IDHM de educacao por estado
- Comparação dos percentuais dos IDHMs de educacao que estão abaixo da média por estado

E por fim, a partir dos dados educacionais coletados e organizados foi proposto uma ordem de priorização para investimento na educação dessa região (Nordeste).

--- 

### Fontes de Dados
Os dados utilizados nesta análise foram extraidos de uma planilha excel dos <a href='https://www.kaggle.com/crisparada/brazilian-cities/downloads/brazilian-cities.zip/6'>IDHM Municipais do Brasil</a> contido na plataforma Kaggle, as colunas analizadas foram: <br>
<code>Município, Estado, IBGE_1-4, IDHM, IDHM_Renda, IDHM_Educacao, GDP_CAPITA, COMP_P</code>

### Ferramentas e Tecnologias 

![image](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)
![image](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
![image](https://img.shields.io/badge/Plotly-239120?style=for-the-badge&logo=plotly&logoColor=white)
![image](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)

### Metodologia
- Coleta de dados: Foi utilizado um arquivo xlsx (excel) para a leitura dos dados e extrair informações sobre municípios, estados, quantidade de crianças de 1 a 4 anos, IDHM, IDHM da renda, IDHM educacional, renda per capta, quantidade de empresas educacionais
- Limpeza de dados: Substituiu valores NaN e Nulos nas colunas por 0
- Análise Exploratória: Visualização dos resultados para uma análise municipal, estadual e regional dos dados. E observar possíveis relações entre os tipos de IDHM e tudo que contempla as suas variações




