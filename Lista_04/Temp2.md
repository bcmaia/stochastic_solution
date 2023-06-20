Temp2


# Questão 11
Seja $\{N(t), t \neq 0\}$ um processo de Poisson de taxa $\lambda$. 
Para $s < t$ encontre:

### (d) $E[N(s)|N(t) = 4]$ (Resp.: 4s/t)

Para calcular esperança, podemos aplicar o somatório:
$$ E[X] = \sum _x x \cdot Pr\{ X = x \}$$

Sabemos que $N(s) \le 4$, então:
$$ E[N(s)|N(t) = 4] 
    = \sum _{i = 0} ^{4} i \cdot Pr\{N(s) = i | N(t) = 4\}
$$

$$ Pr\{N(s) = i | N(t) = 4\} = \frac {e^{-\lambda s}(\lambda s)^i} {i!} $$

$$ E[N(s)|N(t) = 4] 
    = \sum _{i = 0} ^{4} i \cdot \frac {e^{-\lambda s}(\lambda s)^i} {i!}
$$

$$ E[N(s)|N(t) = 4] 
    = e^{-\lambda s} \sum _{i = 0} ^{4} i \cdot \frac {(\lambda s)^i} {i!}
$$

$$ E[N(s)|N(t) = 4] 
    = e^{-\lambda s} [
        0 + \lambda s + \lambda^2 s^2 
        + \frac {\lambda^3 s^3} {2}
        + \frac {\lambda^4 s^4} {6}
    ]
$$