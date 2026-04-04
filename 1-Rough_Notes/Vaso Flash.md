
2026-04-01 22:17

Status: #baby 

Tags: [[Faculdade]] [[Operacoes Unitarias II]]


# Vaso Flash


Um sistema onde dadas Pressao, Temperatura, Composição e Energia. Quanto vira vapor, liquido e qual composição de cada fase

## As variaveis mais importanted do Flash

- Alimentação: F,zi
- Vapor: V,TV,PV,yi
- Líquido: L,TL,PL,xi

Com F,V,L sendo vazoes molares

$$
K_{i} = \frac{y_{i}}{x_{i}}
$$
Sendo essa a Raza de equilíbrio.

$$
\beta = \frac{V}{F}
$$

Sendo essa a Fração vaporizada


## Balanço global de massa

$$
F=L+V
$$

Tudo que entra sair

## Balanço por componente

$$
Fz_{i} = Lx_{i}+Vy_{i}
$$

A quantidade de componente $i$ que entra se divide entre a fase líquida e a fase vapor.




## Equilíbrio entre fases

$$
\begin{aligned}
& T_V=T_L \\
& P_V=P_L \\
& y_i=K_i x_i
\end{aligned}
$$

Ou seja, as duas fases saem na mesma temperatura, mesma pressao e suas composções de relacionam por $K_{i}$



## Introdução a $\beta$




$$
\begin{aligned}
& x_i=\frac{z_i}{(1-\beta)+\beta K_i} \\
& y_i=\frac{z_i K_i}{(1-\beta)+\beta K_i}
\end{aligned}
$$


Apos fazer manipulação de expressões, consegue-se essas formulas que sao centrais para questões de flash

A equação de Flash é então. As frações molares devem somar 1.

$$
\sum_{i=1}^C \frac{z_i\left(1-K_i\right)}{1+\beta\left(K_i-1\right)}=0
$$

Quando $P$, $T$ e $z_{i}$ são conhecidos, o problema vira:

1- Calcular $K_{i}$;
2- Resolver essa equação para $\beta$;
3- Calcular $x_{i}$ e $y_{I}$;
4- Calcular $V$ e $L$.


## O que é $K_{i}$ e como saber se o componente prefere vapor ou líquido.


Para a mistura ideal

$$
K_i=\frac{P_{v a p, i}}{P}
$$

Pela Lei de Raoult

### Se $K_{i}>1$, então:

$$
y_{i}>x_{i}
$$
E o componente prefere a fase vapor




### Se $K_{i}<1$, então:



$$
y_{i}<x_{i}
$$
E o componente prefere a fase líquida.


## Descobrindo a condição física da carga

### Ponto de bolha:

Quando $\beta = 0$:

$$
\sum z_i K_i=1
$$

A mistura está no limite de começar a vaporizar
Está essencialmente líquida, com uma bolha de vapor se formando

### Ponto de orvalho:

Quando $\beta=1$:

$$
\sum \frac{z_i}{K_i}=1
$$

A mistura esta no limite de começar a condensar
Ainda é essencialmente vapor, com uma gota de líquido se formando

### Como usar isso na pratica.

- Avaliar a equação de flash em $\beta=0$, isto é $f(o)$
- Avaliar a equação de flash em $\beta=1$, isto é $f(1)$

Concluindo

- Caso alguns $K_{i}$ sejam maiores que 1 e outros menores que 1, vale a pena testar $f(o)$ e $f(1)$
- Se $f(0)<0$, a mistura esta acima do ponto de bolha
- Se $f(1)>0$, a mistura esta abaixo do ponto de orvalho
- Caso isso acontecem ao mesmo tempo, a carga está dentro da região ELV, então existe solução com $0<\beta<1$.



# References
