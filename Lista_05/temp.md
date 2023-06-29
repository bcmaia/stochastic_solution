* Nessa situação, existem apenas três estados reais: Todas as máquinas estão quebradas, Apenas uma das máquinas está quebrada e Nenhuma das máquinas está quebrada.
    * Isso é: $0, 1, 2$, máquinas funcionando.
* Como há duas máquinas independentes, a taxa de $0 \to 1$ é $2\lambda$ e a de $2 \to 1$ é $2 \mu$.
* Como as máquinas são independentes e não ocorrem dois eventos simultâneos, a taxa de $1 \to 2$ é $\lambda$ e a taxa de $1 \to 0$ é $\mu$.
* Considerando que a distribuição das taxas é exponencial, o tempo médio de transição é $\frac{1}{x}$. Com isso, os tempos médios de transição são:
    * $E[T_0] = \frac{1}{2\lambda}$
    * $E[T_1] = \frac{1}{\lambda + \mu}$
    * $E[T_2] = \frac{1}{2\mu}$
* Como descrito na questão anterior:
    * $P_{01} = 2\lambda$
    * $P_{21} = 2 \mu$
    * $P_{12} = \lambda$
    * $P_{10} = \mu$