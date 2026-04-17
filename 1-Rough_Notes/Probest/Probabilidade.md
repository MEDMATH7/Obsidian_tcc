
2026-04-08 21:24

Status: #baby #portuguse 

Tags: [[Faculdade]] [[Probabilidade e Estatistica]] [[Bloco 1 - Fundamentos de probabilidade ]]

# Probabilidade


## Probabilidade clássica

Define-se como

$$

\begin{align}
P(A) = \frac{|A|}{|\Omega|} \\
\text{probabilidade} = \frac{\text{número de casos favoráveis}}{\text{número total de casos possíveis}}
\end{align}
$$

## Probabilidade condicional

Define-se como:

$$
P(A|B) = \frac{P(A \cap B)}{P(B)}, \quad P(B) > 0
$$

### Intuição de primeiros princípios

Quando eu calculo $P(A)$, estou olhando para o espaço amostral inteiro.
Quando eu calculo $P(A|B).$, eu recebo uma informação nova: **sei que BBB aconteceu**.
Então o universo de possibilidades encolhe.
Agora eu não olho mais para $\Omega$ inteiro. Eu olho apenas para a parte onde BBB aconteceu.
Dentro desse novo universo, pergunto:

“qual fração também pertence a $A$?”

$$
\frac{P(A \cap B)}{P(B)}
$$



### Exemplo:

Lance um dado.

- $A$: sair número par = ${2,4,6}$
- $B$: sair número maior que 3 = ${4,5,6}$


Queremos:

$$
P(A|B)
$$

Primeiro:

$$
A \cap B = \{4,6\}
$$
Logo

$$
\begin{align}
P(B) = \frac{3}{6} \\
P(A \cap B) = \frac{2}{6}
\end{align}
$$

Então

$$
P(A|B) = \frac{\frac{2}{6}}{\frac{3}{6}} = \frac{2}{3}
$$

Sem a condição, a chance de sair par era $\frac{3}{6} = \frac{1}{2}$.
Com a condição “sabemos que saiu número maior que 3”, a chance vira $\frac{2}{3}$.

Ou seja: **a informação mudou a probabilidade**.



# References
