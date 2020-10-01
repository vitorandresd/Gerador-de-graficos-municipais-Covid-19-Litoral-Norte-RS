# Gerador-de-graficos-municipais-Covid-19-Litoral-Norte-RS

Este arquivo utiliza os dados informados no Boletim Coronavírus, enviado pela 18ª Coordenadoria Regional de Saúde do Rio Grande do Sul.
Na primeira planilha do arquivo está a estrutura que dever ser modificada para gerar as informações que gerarão os gráficos das planilhas individuais dos municípios.
A inserção de dados deve ocorrer apenas na planilha chamada DADOS DINÂMICOS.
Obs.: Por falha na informação de testes realizados, o município de Itati precisou de tratamento dos dados e é o único que precisa ser revisto na planilha DADOS. Isso está na Linha 4, colunas G e H.
Na planilha DADOS DINÂMICOS, o procedimento para inserção de dados é a seguinte (vou usar a linguagem própria do Ecxel "Coluna e Linha" para facilitar):
- Na Coluna "A" Linha 1 (A1), informe a quantidade de dias corridos entre o boletim semanal mais antigo e a data da atualização da planilha. Geralmente será 28 dias. Informe apenas o número.
- Em C1 informe a quantidade de dias corridos desde o início da contagem dos dados. Se for utilizar a data inicial dos boletins, é 06/04. Caso for utilizar um período diferente, ajuste a contagem de dias e informe nesse campo.
- Os dados do boletim mais recente devem ser informados por município, da seguinte forma: na coluna D os dados de testes realizados, na coluna N os casos positivos e na coluna X os dados de óbitos. Por padrão, esses valores são dados acumulados no boletim, mas a própria planilha fará a subtração para informar os dados apenas da semana.
Para tanto, é preciso informar os dados das 4 semanas anteriores também.
Isso pode ser feito, para os testes, nas colunas E, G, I e K. Para positivos, nas colunas O, Q, S e U. E para óbitos, nas colunas Y, AA, AC e AE.
Onde indica "semana 1" deve ser informado o que consta no boletim de uma semana atrás, onde diz "semana 2", de duas semanas atrás e assim sucessivamente.
Na sequência há uma planilha para cada município com um dashboard contendo várias informações sobre contágio e comparações com a região.
A metodologia utilizada para a criação dos indicadores é a que segue (extraído de um relatório entregue à AMLINORTE):
Este relatório é resultado da elaboração e análise de indicadores relacionados à Covid-19 no Litoral Norte do Rio Grande Sul. Sua elaboração se dá a partir dos dados
informados pela 18ª Coordenadoria Regional de Saúde do Estado do Rio Grande do Sul (CRS) juntamente do Centro de Operações de Emergências, por meio do Boletim Coronavírus,
publicado todos os dias, de segunda à sexta-feira, com os dados da doença em cada município da região de abrangência.
O trabalho apresentado aqui não pretende ser definitivo em relação às informações apresentadas, mas servir com ferramenta que auxilie a tomada de decisão, especialmente
para a gestão pública, explicitando as diferenças da evolução do transmissão de Sars-Cov-2 (novo coronavírus) que causa Covid19 nos municípios da região.
A partir das comparações entre os municípios em cada um dos indicadores elaborados é possível extrair as principais distinções e compreender o que gera os resultados diferentes
em cada município, bem como elaborar planos de ação para correção de problemas e até mesmo para replicar no território as ações bem sucedidas.
Contribuíram para este trabalho:
Liane Loder, Vítor Duarte, Ricardo Dagnino, Eliseu Weber, Daniela Dietz, Lisiane Lima, Aline Callegaro, Cleo Silveira, Cristiano Hackmann, Lais Zuchetti, Ivone Menegolla, Ana
Cardinale e Maristela Lima.

A partir dos dados de testes realizados, casos positivos e óbitos, em cada município, foram elaborados os seguintes indicadores:

- Positivos por mil por dia TOTAL:
Este indicador serve para compreender e comparar o contágio proporcionalmente ao total de habitantes de cada município, gerando um valor comparável entre municípios com diferentes populações, levando para uma base de mil habitantes. Também se divide pelos dias do intervalo de tempo observado, visando comparar também períodos de tempo diferentes. O "TOTAL" significa que o período analisado é todo (acumulado), contando desde o primeiro dia de observações.
 Fórmula:
(Núm. de testes positivos no período / População do município)*1000 / núm. de dias do período.

- Positivos por mil por dia 4 Semanas:
Este indicador reflete apenas as últimas quatro semanas, objetivando comparar com os dados acumulados.
 Fórmula:
(Núm. de testes positivos no período / População do município)*1000 / núm. de dias do período.

- Deficiência de Testes por mil por dia TOTAL:
Este indicador consiste em testes realizados em cada município e a comparação entre eles, tendo o município com mais testes realizados proporcionalmente (por mil habitantes) como o ideal (100% na escala) e a deficiência se dá pela diferença observada entre os demais e o município com a melhor testagem.
Também foi calculado por mil habitantes e por dia, para poder comparar populações e períodos de tempo distintos. O "TOTAL" indica que são dados acumulados desde o início dos registros.
Fórmula:
a) (Núm. de testes realizados no período / População do município)*1000 / núm.
de dias do período.
b) Maior valor da série obtida com todos os municípios pela fórmula "a" vale
como 100%.
c) 1-(Testes realizados no período / "b")

- Deficiência de testes por mil por dia 4 Semanas:
Elaborado da mesma maneira que o anterior, difere-se apenas porque contempla apenas as últimas 4 semanas. Deve ser comparado com o anterior para auxiliar a compreender se a
testagem vem aumentando ou diminuindo ao longo do tempo.
 Fórmula:
a) (Núm. de testes realizados no período / População do município)*1000 / núm. de dias do período)
b) Maior valor da série obtida com todos os municípios pela fórmula "a" vale como 100%.
 c) 1-(Testes realizados no período / "b")

- Positivos x testes TOTAL:
É um indicador simples, pois consiste em dividir os testes que resultaram positivo pelo total de testes realizados, gerando um percentual de positivos. Com isso, se pode identificar, comparando períodos, se há um aumento ou diminuição da proporção de infectados em relação à testagem.
 Fórmula:
 Núm. de testes positivos / Núm. total de testes realizados 
 
 - Positivos x testes 4 Semanas:
Mesmo indicador anterior, porém aplicado para o período de quatro semanas - últimas quatro semanas.
 Fórmula:
Núm. de testes positivos nas últimas 4 semanas / Núm. total de testes realizados nas últimas 4 semanas

- Óbitos por mil (habitantes):
Este indicador apresenta a proporção de óbitos registrados por Covid-19 em cada município, levando-se em conta a população municipal.
 Fórmula:
 (Núm. de óbitos / População do município)*1000

- Letalidade Aparente:
Indica a proporção de óbitos registrados em relação ao total de testes que resultaram positivo.
 Fórmula:
 Núm. de óbitos registrados / Núm. de casos positivos
 
Por fim, para a elaboração dos gráficos de radar, os dados foram todos colocados em uma escala proporcional comparável. Sendo ao município com o maior valor no indicador em questão aplicado valor 1 e os demais apresentados na mesma proporção, de 0 a 1.
