Para encontrar $E[N(s)|N(t) = 4]$, vamos utilizar as propriedades do processo de Poisson.

Sabemos que o processo de Poisson é caracterizado pela propriedade de incrementos independentes e estacionários. Isso significa que, para qualquer intervalo de tempo $t$, o número de eventos que ocorrem nesse intervalo segue uma distribuição de Poisson com parâmetro $\lambda t$, onde $\lambda$ é a taxa média de ocorrência de eventos por unidade de tempo.

No caso em questão, temos que $N(t) = 4$. Isso implica que, até o tempo $t$, ocorreram exatamente 4 eventos. Agora queremos calcular a expectativa de $N(s)$, dado que já ocorreram 4 eventos até o tempo $t$.

Podemos usar a propriedade de incrementos independentes para separar o processo em dois intervalos: o intervalo de tempo $[0, s]$ e o intervalo de tempo $(s, t]$. O número de eventos no intervalo $[0, s]$ segue uma distribuição de Poisson com parâmetro $\lambda s$, enquanto o número de eventos no intervalo $(s, t]$ segue uma distribuição de Poisson com parâmetro $\lambda (t - s)$. Além disso, esses dois intervalos são independentes.

Dado que já ocorreram 4 eventos no intervalo $(0, t]$, a distribuição condicional de $N(s)$ é uma distribuição de Poisson com parâmetro $\lambda s$, pois o número de eventos no intervalo $[0, s]$ é independente do número de eventos no intervalo $(s, t]$.

Portanto, podemos escrever:

$E[N(s)|N(t) = 4] = E[N(s)] = \lambda s$

Assim, a esperança de $N(s)$, condicionada ao evento de ocorrerem 4 eventos até o tempo $t$, é igual a $\lambda s$.