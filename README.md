**Previsão de casos confimados e óbitos por COVID-19 por região (Portugal)**
===============
Este projeto foi desenvolvido no âmbito da disciplina de Aprendizagem Automática II, que é uma disciplina do 1º ano de Mestrado de Engenharia Informática da Universidade do Minho.
Este trabalho tem como objetivo a criação de um bom modelo de previsão de novos casos confirmados por COVID-19, para cada uma das regiões de Portugal Continental.
Como cada uma das regiões de Portugal Continental tem características distintas, tantos nos dados de novos casos de COVID-19 como climatéricas (dados utilizados neste projeto), encontrar o melhor modelo que responde-se ás características de todas as regiões não foi considerada uma boa estratégia, sendo, por esse motivo, estudado modelos para cada uma das regiões.

**Sobre a equipa**
---------------
A equipa de desenvolvimento é composta apenas pela aluna do 1º ano do Mestrado em Engenharia Informática da Universidade do Minho, Rita Pereira.

**Dataset**
---------------
Os dados utilizados do COVID-19 disponibilizados no link https://github.com/dssg-pt/covid19pt-data que correspondem aos fornecidos diariamente nos boletins disponibilizados pela DGS. Em relação aos dados por região apenas são disponibilizados o número de casos confirmados e de óbitos, sendo esse o motivo pela qual foram os assuntos escolhidos para a modelação. Foram utilizados os dados desde o dia 26 de fevereiro de 2020 até ao dia 20 de junho de 2020. 
Para uma melhor previsão foram utilizados os dados de temperatura fornecidos pelo IPMA, a partir da sua API. No entanto, os dados fornecidos pela API do IPMA apenas estão disponíveis para Portugal Continental pelo que foi o grande motivo para apenas trabalhar com as regiões de Portugal Continental. Por haverem regiões, como a região de Lisboa e Vale do Tejo, que compreende integralmente o distrito de Lisboa, quase a totalidade do distrito de Santarém, cerca da metade do distrito de Setúbal e cerca de um terço do distrito de Leiria, foram considerados como temperatura da região a do concelho mais representativo em termos populacionais. Esta interpolação foi feita porque em Portugal não existe uma diferença considerada de temperatura nas várias regiões.

|  Norte |  Lisboa e Vale do Tejo | Algarve |  Alentejo |  Centro |
|---|---|---|---|---|
|  Porto |  Lisboa |  Faro |  Évora |  Coimbra |

Os datasets utilizados podem ser observados na pasta [Data](https://github.com/xRAFPx/AAII/tree/master/Data).

**Modelos**
---------------
As arquiteturas utilizadas foram ARIMA, SVR, LSTM, RNN e GRU. Para cada região foram criados modelos univariados e multivariados, onde foram utilizados os dados de casos confirmados de COVID-19, mortes por COVID-19 e dados da temperatura (média da mínima e média da máxima observadas em cada um dos dias).

**Resultados**
---------------
Os resultados de cada um dos modelos podem ser observados na pasta [Model Output](https://github.com/xRAFPx/AAII/tree/master/Data/Model%20Output).

