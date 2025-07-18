# Analise de um investimento nas ações da Petrobras
Com uma base de dados composta por ação da Petrobras (PETR4), o valor do petroléo Brent, a taxa Selic, Dólar americano, o indicie Ibovespa e um Investimento. Onde 
Em 02/01/2014 compramos 3 lotes da PETR4 pelo valor total de R$5.025,00, e em 02/01/2024 o valor era de R$11.333,99. Utilizamos a Rede Neural Artificial Recorrente - LSTM para realizar previsões para os próximos 30 dias, não obtivemos resultados satisfatórios. Reduzimos então o horizonte para 10 dias, mas o erro permaneceu elevado. Em testes com períodos de 1 a 3 dias, os resultados foram significativamente melhores.


# Conclusão: 
Quanto maior o horizonte de previsão, maior tende a ser o erro da LSTM. Para previsões de até 1 dia, o modelo apresenta desempenho aceitável. No entanto, ao tentar prever 8 dias à frente, os erros se tornam significativamente elevados.

A proposta inicial era utilizar algoritmos capazes de estimar o retorno de um investimento em prazos de 30, 90 e 180 dias. Contudo, até o momento, modelos como Regressão Linear, Facebook Prophet, LSTM e ARIMA não apresentaram resultados satisfatórios para esses intervalos.

Diante disso, recomenda-se utilizar a LSTM para previsões de até 1 dia, podendo se estender, com cautela, até no máximo 3 dias. Já a Regressão Linear mostrou-se eficaz apenas para a previsão do dia seguinte.

* Previsão de Curto Prazo (10 Dias) com Baixa Precisão
![image](https://github.com/user-attachments/assets/a20753ae-122a-48d9-8734-f6a592ffdeb2)

