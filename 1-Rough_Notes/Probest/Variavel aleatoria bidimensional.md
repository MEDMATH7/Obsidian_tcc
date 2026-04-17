
2026-04-16 20:14

Status:

Tags: [[Faculdade]] [[Probabilidade e Estatistica]] [[Bloco 3 - Variaveis aleatorias bidimensionais discretas e dependencia]] 



# Variavel aleatoria bidimensional

Os slides dizem que, se $X$ e $Y$ são variáveis aleatórias definidas no mesmo espaço amostral, então o par $(X,Y)$ é chamado de **vetor aleatório bidimensional**. Se $X$ e $Y$ são discretas, então $(X,Y)$é um vetor aleatório discreto



## Distribuição conjunta

Os slides definem a **função massa de probabilidade conjunta** por

$$
p_{X,Y}(x,y) = P(X = x, Y = y)
$$

para todo $(x,y)$ possível.

Essa é a probabilidade de as duas coisas acontecerem ao mesmo tempo:

$$
\begin{align}

X \text{ assumir valor } x;  \\


\text{e } Y \text{ assumir valor } y.

\end{align}

$$
### Propriedades fundamentais

A função conjunta precisa obedecer:

$$
\begin{align}

p_{X,Y}(x,y) \geq 0  \\


\sum_{x} \sum_{y} p_{X,Y}(x,y) = 1

\end{align}
$$

porque todas as probabilidades têm que ser não negativas e a soma de todos os casos possíveis precisa dar 1

## Distribuições marginais

Os slides definem a marginal de $X$ e $Y$ como


$$
\begin{align}

p_X(x) = \sum_{y} P(X = x, Y = y)  \\


p_Y(y) = \sum_{x} P(X = x, Y = y)

\end{align}
$$

### Intuição real

A marginal é o que sobra quando você “esquece” a outra variável.

Se eu quero saber só como $X$ se comporta, sem me importar com $Y$, eu somo todas as probabilidades conjuntas associadas àquele valor de $X$.

É como dizer:

“qual é a probabilidade de $X=x$, não importa quanto vale $Y$?”

Então:

$$
P(X = x) = \sum_{y} P(X = x, Y = y)
$$
Isso é extremamente importante.

Porque a distribuição conjunta contém mais informação do que as marginais.  
As marginais te dizem o comportamento individual de cada variável.  
A conjunta te diz como elas se comportam **juntas**.

# References
