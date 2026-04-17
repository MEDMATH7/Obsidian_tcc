
2026-04-16 20:46

Status: #baby #portuguse 

Tags: [[Faculdade]] [[Probabilidade e Estatistica]] [[Bloco 3 - Variaveis aleatorias bidimensionais discretas e dependencia]] 



# Independencia entre variaveis aleatorias

Os slides definem que duas variáveis aleatórias discretas $X$ e $Y$ são independentes se
$$
P(X = x, Y = y) = P(X = x)P(Y = y)
$$

para todo $x$ e $y$:

$$
p_{X,Y}(x,y) = p_X(x)p_Y(y)
$$

## Intuição

Independência entre variáveis aleatórias significa:

**saber o valor de uma não muda o comportamento probabilístico da outra.**

Isso é a versão, para variáveis, da ideia de independência que você viu no Bloco 1 para eventos.


### Verificando no exemplo

Temos:

$$
p_{X,Y}(0,1) = 0
$$

mas, se fossem independentes, teríamos que valer:

$$
\begin{align}

p_X(0)p_Y(1) = \frac{1}{2} \cdot \frac{1}{4} = \frac{1}{8}  \\
\text{Como:} \\


0 \neq \frac{1}{8}

\end{align}
$$
então $X$ e $Y$ **não são independentes**.


### Interpretação intuitiva

Se você sabe que $Y=1$, então automaticamente $X$ não pode ser $0$, porque a célula $(0,1)$ tem probabilidade zero.

Ou seja: o valor de $Y$ te dá informação sobre $X$.

Logo, elas não podem ser independentes.


# References
