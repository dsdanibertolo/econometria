# econometria
Neste repositório contém meus estudos de Econometria com dados da Economia Brasileira.

Nele foram usados dados trimestrais do PIB nacional começando do primeiro trimestre de 1966 até o quarto trimestre de 1985 num total de 80 observações.

O modelo tem como variável dependente(exógena) a demanda por encaixes monetários reais (M1) e as variáveis independentes(endógenas), o PIB Real representado por Y (quando se desconta a inflação),a taxa de juros nominal(R) e a taxa de inflação(PI)

Os resultados foram obtidos usando biblioteca statsmodel em Python, o modelo é não linear nas variáveis originais, mas linear na forma logarítmica. Assim, foi usado o método Mínimos Quadrados Ordinários(MQO) ou em inglês Least Squares(LS)
