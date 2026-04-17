
2026-04-14 22:12

Status: #baby #portuguse 

Tags: [[Faculdade]] [[Probabilidade e Estatistica]] [[Bloco 2 - Variáveis aleatórias discretas e distribuições clássicas]]


# Modelo Binomial


Variável aleatória Binomial

$$
P(X = x) = \binom{n}{x} p^x (1 - p)^{n-x}, \quad x = 0, 1, \dots, n
$$

com notação


$$
X \sim Bin(n,p)
$$

e observam que esse modelo surge quando $X$ é o **número de sucessos em nnn ensaios de Bernoulli independentes** com probabilidade $p$ de sucesso


## Intuição de primeiros princípios

A Binomial conta:

**quantos sucessos aconteceram ao repetir várias vezes um experimento Bernoulli independente**.

Essa frase é central.

A Binomial aparece quando temos:

1. número fixo de repetições: $n$;
2. cada repetição tem só sucesso/fracasso;
3. a probabilidade de sucesso é a mesma em todas: $p$;
4. as repetições são independentes.

### Significado de cada termo

$$
\binom{n}{x}
$$

é o número de maneiras de distribuir $x$ sucessos em $n$ tentativas.

$$
p^x
$$
é a probabilidade de ocorrerem exatamente os $x$ sucessos.

$$
(1 - p)^{n-x}
$$

é a probabilidade dos $n-x$ fracassos.

Então a fórmula inteira junta:

- quantas sequências são possíveis;
- probabilidade de cada sequência.

### Exemplo concreto

Se você lança 5 moedas honestas e quer saber a probabilidade de sair exatamente 3 caras, então:

$$
\begin{align}

n = 5  \\


p = 0,5  \\


x = 3

\end{align}
$$

Logo:

$$

\begin{align}

P(X = 3) = \binom{5}{3} (0,5)^3 (0,5)^2  \\


P(X = 3) = 10(0,5)^5  \\


P(X = 3) = 10 \cdot \frac{1}{32}  \\


P(X = 3) = \frac{10}{32} = \frac{5}{16} = 0,3125

\end{align}




$$


# References
