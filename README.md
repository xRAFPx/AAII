**Previsão de casos confimados e óbitos por COVID-19 por região (Portugal)**
===============
Este projeto foi desenvolvido no âmbito da disciplina de Aprendizagem Automática II, que é uma disciplina do 1º ano de Mestrado de Engenharia Informática da Universidade do Minho.
Este trabalho tem como objetivo a criação de um bom modelo de previsão de novos casos confirmados por COVID-19, para cada uma das regiões de Portugal Continental e Ilhas (Açores e Madeira).

**Sobre a equipa**
---------------
A equipa de desenvolvimento é composta apenas pela aluna do 1º ano do Mestrado em Engenharia Informática da Universidade do Minho, Rita Pereira.

**Dataset**
---------------
Os dados utilizados do COVID-19 os disponibilizados no link https://github.com/dssg-pt/covid19pt-data que correspondem aos fornecidos diariamente nos boletins disponibilizados pela DGS. Em relação aos dados por região apenas são disponibilizados o número de casos confirmados e de óbitos, sendo esse o motivo pela qual foram os assuntos escolhidos para a modelação.
Para uma melhor previsão foram utilizados os dados de temperatura fornecidos pelo IPMA, a partir da sua API. No entanto, os dados fornecidos pela API do IPMA apenas estão disponíveis para Portugal Continental pelo que apenas serão usados para prever nas regiões de Portugal Continental. Por haverem regiões, como a região de Lisboa e Vale do Tejo, que compreende integralmente o distrito de Lisboa, quase a totalidade do distrito de Santarém, cerca da metade do distrito de Setúbal e cerca de um terço do distrito de Leiria, foram considerados como temperatura da região a do concelho mais representativo em termos populacionais. Esta interpolação foi feita porque em Portugal não existe uma diferença considerada de temperatura nas várias regiões.

|  Norte |  Lisboa e Vale do Tejo | Algarve |  Alentejo |  Centro |
|---|---|---|---|---|
|  Porto |  Lisboa |  Faro |  Évora |  Coimbra |

Os datasets utilizados podem ser observados na pasta Data.

**Modelos**
---------------
As arquiteturas utilizadas foram ARIMA, SVR, LSTM, RNN e GRU.
