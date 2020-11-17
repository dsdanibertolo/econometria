# econometria
Neste repositório contém meus estudos de Econometria com dados da Economia Brasileira.

Nele foram usados dados trimestrais do PIB nacional começando do primeiro trimestre de 1966 até o quarto trimestre de 1985 num total de 80 observações.

O modelo tem como variável dependente(exógena) a demanda por encaixes monetários reais (M1) e as variáveis independentes(endógenas), o PIB Real representado por Y (quando se desconta a inflação),a taxa de juros nominal(R) e a taxa de inflação(PI)

Para o leitor leigo, explico que M1 é uma representação dos diferentes tipos de moeda no sistema econômico. M1 é a soma de todo papel-moeda e moeda metálica em poder do público mais depósitos à vista nos bancos comerciais. É o tipo de moeda que tem maior liquidez na economia.

## Explicando os resultados obtidos:

Os resultados foram obtidos usando biblioteca statsmodel em Python, o modelo é não linear nas variáveis originais, mas linear na forma logarítmica. Assim, foi usado o método Mínimos Quadrados Ordinários(MQO) ou em inglês Least Squares(LS). Vale acrescentar que o layout dos resultados é bem semelhante à do e-views (para aqueles que não conhecem a ferramenta). A forma logarítmica nos fornece a variação percentual na variável dependente de uma variação de 1% no regressor.


A elasticidade-renda de M1 foi de 0,95 e as elasticidades do agregados monetários reais em relação à taxa de juros e a taxa de inflação foram -0,50 e -0,84 ,respectivamente. O ajustamento do modelo é dado pelo coeficiente de determinação 0,95. Um bom resultado.

Sendo o teste F um teste de significância global de todos os regressores juntos e seu p-valor nesta estimação menor que a significância, aqui podemos rejeitar a hipótese nula e aceitar que o modelo tem um bom ajuste.

Diferente do teste F, o teste T avalia cada regressor, e o p-valor dos testes T para cada um dos regressores menores que a significância,rejeitamos a hipótese nula também.
 
O coeficiente de determinação, também chamado de R2 (ou R-Quadrado)é uma medida de ajuste do modelo estatístico e seu valor varia de 0 a 1.R-quadrado = Variação explicada/Variação total.  Quanto maior seu valor maior mais explitativo é o modelo. Na estimação em questão temos R2 igual a 0,954 ou de outra forma: 95%. Logo,o modelo explica 95% da variância da variável dependente(M1) em relação ao PIB, Juros e Inflação. 

Sobre a variável dummy inserida, esta foi colocada apenas na última observação para fins de teste, com isto confirmamos que mesmo na última observação uma variável dummy força a regressão a passar por ela. Nas estimações das tabelas 1.2 e 1.3 em questão o uso da variável dummy não alterou os valores dos regressores, mexeu muito pouco nos coeficientes de determinação e nos valores dos testes F e T. Não alterou portando a conclusão dos testes de hipóteses.

O uso de uma variável dummy pode auxiliar o analista numa estimação onde se faz estudos sócio-econômicos por exemplo: tem água encanada? Tem Internet? Se sim inserimos 1 se não inserimos 0. 
