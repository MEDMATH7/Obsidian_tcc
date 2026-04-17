
2026-04-14 21:29

Status: #baby #portuguse 

Tags: [[Faculdade]] [[Probabilidade e Estatistica]] [[Bloco 2 - Variáveis aleatórias discretas e distribuições clássicas]]


# variavel aleatoria

Os slides definem variável aleatória como uma **função do espaço amostral em $\mathbb{R}$, isto é, uma regra que pega cada resultado possível do experimento e associa a ele um número real. Os slides também dizem que variáveis aleatórias fornecem “resumos numéricos” de um experimento aleatório

Essa definição parece abstrata no começo, então vamos destrinchar.

### Ideia intuitiva

Você tem:

- um experimento aleatório;
- vários resultados possíveis;
- e quer resumir esses resultados por um número.

A variável aleatória faz exatamente isso.

### Exemplo simples

Suponha 3 lançamentos de moeda.

O espaço amostral poderia ser algo como:

$$
\Omega = \{CCC, CCK, CKC, KCC, CKK, KCK, KKC, KKK\}
$$

onde
$$
\begin{align}
C = cara \\
K=coroa \\
X = \text{ numero de caras em 3 lanc​amentos}
\end{align}
$$

logo

$$
\begin{align}

X(CCC) = 3  \\


X(CCK) = 2  \\


X(CKK) = 1  \\


X(KKK) = 0

\end{align}
$$


Repare no que aconteceu:

o experimento tinha resultados “textuais”, como $CCK$, mas a variável aleatória transformou isso em um número.

Isso é exatamente a ideia dos slides.


## Eventos e variável aleatória



Os slides mostram que, para uma variável aleatória $X$, expressões como {X=x}, {X≤x} e {X≥x} ainda são **eventos**


Porque significa que variável aleatória e evento não são coisas separadas; eles se conectam.

Por exemplo:


$$
\begin{align}

\{X = 2\} \text{ significa "o evento em que a variável aleatória assume valor 2".}  \\


\{X \geq 1\} \text{ significa "o evento em que a variável assume valor pelo menos 1".}

\end{align}
$$


Ou seja: a variável aleatória cria uma ponte entre **probabilidade de eventos** e **probabilidade de valores numéricos**.


## Variável aleatória discreta e função massa de probabilidade


Os slides definem que uma variável aleatória é **discreta** quando assume valores em um conjunto enumerável, e sua **função massa de probabilidade** é

$$
p_X(x) = P(X = x)
$$

Alem disso, a função massa deve satisfazer:

$$
\begin{align}

p_X(x) \geq 0  \\

\text{ e } \\

\sum_{x \in \Omega_X} p_X(x) = 1

\end{align}
$$


### O que isso quer dizer na prática?

Se $X$ é discreta, então ela assume valores “separados”, como:

- 0, 1, 2, 3;
- ou 0 e 1;
- ou 0, 1, 2, 3, 4, ...

E para cada valor possível, existe uma probabilidade associada.

A função massa é basicamente uma tabela:

- valor possível;
- probabilidade desse valor.

### Exemplo

Se $X$ for o número de caras em 2 lançamentos de moeda honesta, então os valores possíveis são:

$$
\Omega_X = {0, 1, 2}
$$

A função massa é:

$$
P(X = 0) = \frac{1}{4}, \quad P(X = 1) = \frac{1}{2}, \quad P(X = 2) = \frac{1}{4}
$$

a soma dá 1.


# References
