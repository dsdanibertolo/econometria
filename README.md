# econometria
Neste repositório contém meus estudos de Econometria com dados da Economia Brasileira.

Nele foram usados dados trimestrais do PIB nacional começando do primeiro trimestre de 1966 até o quarto trimestre de 1985 num total de 80 observações.

O modelo tem como variável dependente(exógena) a demanda por encaixes monetários reais (M1) e as variáveis independentes(endógenas), o PIB Real representado por Y (quando se desconta a inflação),a taxa de juros nominal(R) e a taxa de inflação(PI)

## Explicando os resultados obtidos:

Os resultados foram obtidos usando biblioteca statsmodel em Python, o modelo é não linear nas variáveis originais, mas linear na forma logarítmica. Assim, foi usado o método Mínimos Quadrados Ordinários(MQO) ou em inglês Least Squares(LS). Vale acrescentar que o layout dos resultados é bem semelhante à do e-views (para aqueles que não conhecem a ferramenta). 

A elasticidade-renda de M1 foi de 0,95 e as elasticidades do agregados monetários reais em relação à taxa de juros e a taxa de inflação foram -0,50 e -0,84 ,respectivamente. O ajustamento do modelo é dado pelo coeficiente de determinação 0,95. Um bom resultado.

Sendo o teste F um teste de significância global de todos os regressores juntos e seu p-valor nesta estimação menor que a significância, aqui podemos rejeitar a hipótese nula e aceitar que o modelo tem um bom ajuste.

Diferente do teste F, o teste T avalia cada regressor, e o p-valor dos testes T para cada um dos regressores menores que a significância,rejeitamos a hipótese nula também.
 
