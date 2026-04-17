
2026-04-16 20:53

Status: #baby #portuguse 

Tags: [[Faculdade]] [[Probabilidade e Estatistica]] [[Bloco 3 - Variaveis aleatorias bidimensionais discretas e dependencia]] 


# Distribuicao condicional


Na Aula 6, os slides definem a função massa condicional de $X$ dado $Y=y$ como


$$
p_{X|Y}(x|y) = \frac{p_{X,Y}(x,y)}{p_Y(y)}
$$
desde que $py(y)>0$


## Intuição

Agora a lógica é muito parecida com a probabilidade condicional do Bloco 1.

Só que, em vez de condicionar por um evento genérico, você condiciona pelo fato de uma variável ter assumido certo valor.

Em outras palavras:

“se eu souber que $Y=y$, como fica a distribuição de $X$?”

Você está restringindo o universo aos casos em que $Y=y$.

## Calculando $X∣Y=0$ no exemplo

Sabemos que:

$$
py(0) = \frac{3}{4}
$$
Então:

para $x=0$

$$
p_{X|Y}(0|0) = \frac{p_{X,Y}(0,0)}{p_Y(0)} = \frac{1/2}{3/4} = \frac{2}{3}
$$


para $x=1$

$$
p_{X|Y}(1|0) = \frac{p_{X,Y}(1,0)}{p_Y(0)} = \frac{1/4}{3/4} = \frac{1}{3}
$$

Logo:

$$
P(X = 0|Y = 0) = \frac{2}{3}, \quad P(X = 1|Y = 0) = \frac{1}{3}
$$

## Calculando $X∣Y=1$


Sabemos que:

Sabemos que

$$
py(0) = \frac{1}{4}
$$

Então

Para $x=0$

$$
p_{X|Y}(0|1) = \frac{p_{X,Y}(0,1)}{p_Y(1)} = \frac{0}{1/4} = 0
$$
Para $x=1$

$$
p_{X|Y}(1|1) = \frac{p_{X,Y}(1,1)}{p_Y(1)} = \frac{1/4}{1/4} = 1
$$

Logo:

$$
P(X = 0|Y = 1) = 0, \quad P(X = 1|Y = 1) = 1
$$

Interpretação:

se $Y=1$, então $X$ obrigatoriamente vale 1.


# References
