## Covid-19: Uma criança de 0 a 4 anos de idade morreu por semana no Ceará

Nos mais de dois anos de pandemia, a Covid-19 deixa um rastro de dor e sofrimento com mais de 670 mil mortes no Brasil. Somente no Ceará, 27 mil morreram em decorrência da contaminação pelo vírus. Deste total de mortes no Estado, 151 óbitos ocorreram entre crianças de 0 a 4 anos, no período de 2020 até 18 de julho de 2022.

Dos 151 óbitos registrados no Estado até o momento, 138 (91,4%) ocorreram entre as crianças de 0 a 2 anos; já entre as de 3 e 4 anos, foram 13 (8,6%). Considerando o mesmo período (1º/1 a 11/7) nos anos de 2020, 2021 e 2022, o ano com mais óbitos nesta faixa etária foi o último. A faixa etária com maior mortalidade é a única para a qual ainda não existem vacinas liberadas, [desde que a imunização de crianças de 3 a 5 anos foi liberada no Ceará, em 18 de julho](https://www.opovo.com.br/coronavirus/2022/07/15/covid-19-vacinacao-de-criancas-de-3-a-5-anos-em-fortaleza-vai-acontecer-sem-agendamento.html).

Em um contexto de politização em torno da vacina contra a Covid-19, em especial quando se fala da faixa etária mais jovem, é essencial que o jornalismo continue acompanhando o desenrolar da pandemia e os impactos que a doença causa na população. Foi pensando nisso que a Central de Jornalismo de Dados do Jornal O POVO (DATADOC) e o Núcleo de Cotidiano do O POVO uniram-se para a realização da reportagem [Covid-19: Uma criança de 0 a 4 anos de idade morreu por semana no Ceará](https://mais.opovo.com.br/reportagens-especiais/2022/07/29/covid-19-uma-crianca-de-0-a-4-anos-de-idade-morreu-por-semana-no-ceara.html), publicada na sexta-feira, 29 de julho de 2022.

Neste repositório, é possível encontrar os códigos para coleta via API da plataforma IntegraSUS e análise dos dados referentes aos óbitos por Covid-19 entre crianças menores de 5 anos no Ceará. A análise foi feita pela DATADOC e o texto, assinado pelo repórter Gabriel Borges.

![Acumulado de óbitos por Covid-19 em crianças de 0 a 4 anos no Ceará, de 2020 a 18 de julho de 2022](imagem/acumulado.png)

--------------------------------------

### Fonte e coleta de dados:

- [Boletim Covid-19, no IntegraSUS, plataforma da Secretaria da Saúde do Estado do Ceará (Sesa)](https://integrasus.saude.ce.gov.br/#/indicadores/indicadores-coronavirus/coronavirus-ceara)

### Metodologia

Inicialmente, foram raspados os dados de óbitos por Covid-19 no Ceará, por faixa etária, desde o início de 2020 até 18 de julho de 2022. Esse arquivo foi salvo como `20220718_df_obitos_por_idade.csv`. Em seguida, foram filtrados os óbitos entre crianças de 0 a 2 anos e de 3 a 4 anos de idade.

Com esse filtro, foram calculados os óbitos nessas idades por ano (2020, 2021 e 2022 — nesse último caso, até 18 de julho) e no período de 1º de janeiro a 18 de julho de cada um desses anos, além do percentual representado pelas faixas etárias (0 a 2 anos e 3 a 4 anos) nesses óbitos pela doença até o momento da análise.

### Arquivos gerados:

**_Dataframes_**
 - `20220718_df_obitos_00_04_acumulados_grafico.csv`:  Acumulado de óbitos por Covid-19 em crianças de 0 a 4 anos, no Ceará, de 1º de janeiro de 2020 a 18 de julho de 2022 ;
 - `20220718_df_obitos_00_04_comp_anos.csv`:  Óbitos por Covid-19 em crianças de 0 a 4 anos, no Ceará, por faixa etária, divididos por ano e por período (1º/jan a 18/jul).
 
 **_Visualizações_**
- [Acumulado de óbitos por Covid-19 em crianças de 0 a 4 anos no Ceará](https://public.flourish.studio/visualisation/10527332/)
- [Óbitos por Covid-19 no Ceará em crianças de 0 a 4 anos, por faixa etária e ano](https://public.flourish.studio/visualisation/10527141/)

--------------------------------------

#### Como utilizar:

Para executar o notebook com a coleta e processamento dos dados, é necessário um ambiente com *Python3* e dependências que podem ser instaladas via [Pip](https://pypi.org/project/pip/): 
```{python}
!pip install pandas
!pip install numpy
!pip install DateTime
```

### A central DATADOC

A Central de Jornalismo de Dados do O POVO (DATADOC) alia tecnologia e técnicas diversas de análises de dados para produzir um jornalismo de precisão para que você forme sua opinião com segurança. Nosso objetivo é fazer com que todos tenham acesso aos dados utilizados nas notícias que produzimos.

A DATADOC é composta por uma equipe de três jornalistas (sendo uma infografista), uma desenvolvedora front-end e um cientista da computação que coletam, enriquecem e disponibilizam as bases e códigos de cada reportagem para um jornalismo transparente e baseado em evidências.

 --------------------------------------
#### 🔥📰👩🏻‍💻 Se você gostou do nosso material, apoie assinando o OP+ e acompanhando o nosso trabalho.

#### 📝📨 Para feedback, dúvidas ou sugestões: datadoc@opovodigital.com

--------------------------------------
 
🎤🎼 Confira também outras produções recentes da central DATADOC: A matéria  ***Gilberto Gil 80 anos: uma viagem pelas composições e parcerias do baiano*** mostrou análises de composições e estatísticas das produções do artista nas plataformas YouTube e Spotify. A matéria está [disponível no O POVO Online](https://www.opovo.com.br/vidaearte/2022/06/24/gilberto-gil-80-anos-uma-viagem-pelas-composicoes-e-parcerias-do-baiano.html).
