temp 4

Para encontrar $E[N(s)|N(t) = 4]$, usaremos a propriedade da propriedade de incrementos independentes do processo de Poisson.

Sabemos que o processo de Poisson tem a propriedade de incrementos independentes, o que significa que o número de ocorrências em intervalos não sobrepostos é independente. Portanto, podemos considerar o intervalo $[s, t]$ como um único intervalo.

A distribuição do processo de Poisson é dada por $N(t) \sim \text{Poisson}(\lambda t)$, onde $\lambda$ é a taxa de chegada.

A média e a variância de uma distribuição de Poisson são iguais à taxa $\lambda$. Portanto, a média e a variância de $N(t)$ são $\lambda t$.

Queremos encontrar $E[N(s)|N(t) = 4]$, ou seja, a média condicional de $N(s)$ dado que $N(t) = 4$. 

Usando a propriedade da propriedade de incrementos independentes, podemos escrever:

$N(t) - N(s) \sim \text{Poisson}(\lambda (t - s))$

Dado que $N(t) = 4$, temos:

$4 - N(s) \sim \text{Poisson}(\lambda (t - s))$

Agora podemos calcular a média condicional utilizando a definição da distribuição de Poisson:

$E[4 - N(s)] = 4 - E[N(s)] = \lambda (t - s)$

Rearranjando a equação, obtemos:

$E[N(s)] = 4 - \lambda (t - s)$

Portanto, $E[N(s)|N(t) = 4] = 4 - \lambda (t - s)$.