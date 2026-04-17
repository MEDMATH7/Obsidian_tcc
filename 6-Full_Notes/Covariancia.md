
2026-04-16 21:13

Status: #baby #portuguse 

Tags: [[Faculdade]] [[Probabilidade e Estatistica]] [[Bloco 3 - Variaveis aleatorias bidimensionais discretas e dependencia]] 


# Covariancia

Os slides definem a covariância por

$$
Cov(X, Y) = E[(X - E(X))(Y - E(Y))]
$$

E também

$$
Cov(X, Y) = E(XY) - E(X)E(Y)
$$

## Intuição física

A covariância mede se $X$ e $Y$ tendem a variar juntas.

- se, quando $X$ fica maior, $Y$ também tende a ficar maior, a covariância tende a ser positiva;
- se, quando $X$ fica maior, $Y$ tende a ficar menor, a covariância tende a ser negativa;
- se não há tendência linear clara, ela pode ficar próxima de zero.

Mas cuidado:
**covariância zero não significa automaticamente independência**.

Independência implica covariância zero em muitos contextos do curso, mas o contrário não é sempre verdadeiro.

Os slides também lembram que, se  $X$ e $Y$ são independentes, então $Cov(X,Y)=0$.
## Calculando a covariância no exemplo

Vamos calcular tudo passo a passo.

Passo 1: calcular $E(X)$

como $X \sim Ber(1/2):$ 

$$
E(X) = \frac{1}{2}
$$


Passo 2: calcular $E(X)$

como $X \sim Ber(1/4):$ 

$$
E(Y) = \frac{1}{4}
$$

### Passo 3: calcular $E(XY)$

Precisamos somar $xy p_{X,Y}(x,y)$ para todos os pares possíveis.

$$
\begin{align} \text{se } (x,y) = (0, 0), \text{ então } xy = 0  \\
 \text{se } (0, 1), \text{ então } xy = 0  \\
 \text{se } (1, 0), \text{ então } xy = 0  \\
  \text{se } (1, 1), \text{ então } xy = 1 \end{align}
$$
Logo:

$$
E(XY) = 0 \cdot \frac{1}{2} + 0 \cdot 0 + 0 \cdot \frac{1}{4} + 1 \cdot \frac{1}{4} = \frac{1}{4}
$$
### Passo 4: aplicar a fórmula


$$
\begin{align}

Cov(X, Y) = E(XY) - E(X)E(Y)  \\


Cov(X, Y) = \frac{1}{4} - \frac{1}{2} \cdot \frac{1}{4}  \\


Cov(X, Y) = \frac{1}{4} - \frac{1}{8} = \frac{1}{8}

\end{align}


$$

Resultado

$$
Cov(X, Y) = \frac{1}{8}
$$

Como é positiva, isso sugere que valores maiores de $X$ tendem a aparecer com valores maiores de $Y$, o que faz sentido nesse exemplo.


# References
