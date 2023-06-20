Temp

## Questão 11
Seja $\{N(t), t \neq 0\}$ um processo de Poisson de taxa $\lambda$. 
Para $s < t$ encontre:

### (d) $E[N(s)|N(t) = 4]$ (Resp.: 4s/t)

Para calcular esperança, podemos aplicar o somatório:
$$ E[X] = \sum _x x \cdot Pr\{ X = x \}$$

Note que, como s e t não são intervalos disjuntos, 
precisamos usar a propriedade de incrementos independentes do 
processo de Poisson:
$$ E[N(s)|N(t) = 4] 
    = \sum _{i = 0} ^{4} (4 - i) \cdot Pr\{N(t) - N(s) = i | N(t) = 4\}
$$

Aqui, $(4-i)$ representa o valor que $N(s)$ assume em cada caso,
e $Pr{N(t)-N(s) = i | N(t) = 4}$ representa a probabilidade desse caso ocorrer,
dado que $N(t) = 4$.

Aplicando a formula de probabilidade condicional, obtemos
$$ E[N(s)|N(t) = 4] 
    = \sum _{i = 0} ^{4} (4 - i) 
        \cdot \frac {
                Pr\{N(t) - N(s) = i\} \cdot Pr\{N(t) = 4\}
            } {
                Pr\{N(t) = 4\}
            }
$$

Podemos calcular essas probavilidades da seguinte forma
$$ Pr\{N(t) = 4\} = \frac {e^{-\lambda t} \cdot (\lambda t)^4} {4!} $$
$$ Pr\{N(t) - N(s) = i\} 
    = \frac {e^{-\lambda(t-s)} \cdot [\lambda(t-s)]^i} {i!} 
$$

Agora, substituindo essas informações na expressão para E[N(s)|N(t) = 4], temos:
$$
    E[N(s)|N(t) = 4] 
        = \sum _{i = 0} ^{4} 
            (4 - i) * \frac {
                Pr\{ N(t) - N(s) = i \} * Pr\{ N(t) = 4 \}
            } {
                Pr\{ N(t) = 4 \}
            }
$$


$$ E[N(s)|N(t) = 4] 
    = \sum _{i = 0} ^{4} 
        (4 - i) 
        \cdot \frac {
            e^{-\lambda(t-s)} 
            \cdot [\lambda(t-s)]^i 
            \cdot e^{-\lambda t} 
            \cdot (\lambda t)^4
        } {
            i! \cdot 4!
        } 
$$

Simplificando a expressão:
$$ E[N(s)|N(t) = 4] 
    = \frac {
        e^{-\lambda(t-s)} \cdot e^{-\lambda t} \cdot (\lambda t)^4
    } {4!} 
    \sum _{i = 0} ^{4} \frac { (4 - i) \cdot [\lambda(t-s)]^i } { i! } 
$$

ERROR 
$$ \error $$

Portanto, temos:
$$ 
    E[N(s)|N(t) = 4] 
        = \frac {e^{-\lambda(t-s)} \cdot e^{-\lambda t} \cdot (\lambda t)^4} {4!} \cdot (\lambda(t-s) + 1)^4 
$$

Simplificando ainda mais:
$$ E[N(s)|N(t) = 4] 
    = \frac {
        e^{-\lambda(t-s)} \cdot (\lambda t)^4
    } {
        4!
    } \cdot (\lambda(t-s) + 1)^4 
$$

<br>

Assim, chegamos a
> .
> $$ E[N(s)|N(t) = 4] = \frac {4s} {t} $$
> .




