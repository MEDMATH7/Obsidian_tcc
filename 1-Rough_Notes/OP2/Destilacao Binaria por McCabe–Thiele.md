
2026-04-09 20:10

Status: #baby #portuguse 

Tags: [[Faculdade]] [[Operacoes Unitarias II]] 


# Destilacao Binaria por McCabe–Thiele

Uma coluna de destilação binária pode ser pensada como uma sequência de estágios de equilíbrio.

Em cada estágio:

- o vapor sobe, mais rico no componente mais volátil;
- o líquido desce, mais rico no menos volátil;
- eles entram em contato e saem em equilíbrio.

O método de McCabe–Thiele transforma isso num problema gráfico no plano:

$$
x \text{ versus } y

$$


onde

$$
\begin{align}
x=\text{composição do componente mais volátil na fase líquida} \\
y = \text{composição do componente mais volátil na fase vapor.}
\end{align}
$$

O diagrama sempre tem:

- a **curva de equilíbrio**;
- a **diagonal** $y=x$;
- as **retas de operação**;
- e a reta $q$ da alimentação.

A partir disso, você “sobe e anda” no gráfico para contar estágios.

## Seções da coluna

Temos a seção de topo de **seção de absorção** e a de baixo de **seção de esgotamento**. No contexto de destilação, você pode interpretar assim:

- **Seção de absorção / retificação / enriquecimento**: região acima da alimentação, onde o vapor vai ficando mais rico no componente mais volátil.
- **Seção de esgotamento**: região abaixo da alimentação, onde o líquido vai ficando mais pobre no componente mais volátil.

Essas duas seções têm retas de operação diferentes.

## Curva de equilíbrio e diagonal $y=x$


Antes de qualquer coisa, você precisa do diagrama de equilíbrio $xy$ .

Se o sistema for ideal e a volatilidade relativa $\alpha$ puder ser considerada constante, vale:

$$
y = \frac{\alpha x}{1 + x(\alpha - 1)}
$$


Esse tipo de relação aparece nos exemplos de destilação binária e é a base para construir a curva de equilíbrio.

A diagonal:

$$
y=x
$$


## Reta de operação da seção de topo: R.O.S.A

A partir do balanço molar na seção de topo temos:

$$
y_n = \frac{L}{V}x_{n-1} + \frac{D}{V}x_D
$$

e usando a razão de refluxo externa de topo:
$$
RR=\frac{L_0}{D}
$$
e a relação $V=L+D$ chega-se em

$$
y = \frac{RR}{RR + 1}x + \frac{x_D}{RR + 1}
$$

Essa é a **reta de operação da seção de absorção**.


### Intuição física

Se você aumenta $RR$, aumenta o líquido que retorna como refluxo. Isso “puxa” a reta de operação para mais perto da diagonal e melhora a separação, mas custa mais energia.


## Reta de operação da seção de fundo: R.O.S.E.

Para a seção de esgotamento, a professora obtém:

$$
y_m = \frac{\bar{L}}{\bar{V}}x_{m-1} - \frac{B}{\bar{V}}x_B
$$

Essa é a **reta de operação da seção de esgotamento**
### Interpretação

- $x_{B}$​: composição do produto de fundo.
- ela passa pela diagonal no ponto:
$$
y=x=x_{B}
$$

Isso é muito útil graficamente: para desenhar a R.O.S.E., um ponto importante já é o ponto $(x_{B},x_{B})$



## A reta q

A reta q representa o **lugar geométrico das possíveis interseções entre a reta de topo e a reta de fundo**. Em uma coluna com uma alimentação e sem retiradas laterais, essa interseção acontece no **estágio de carga**.

Define-se
$$
q = \frac{\bar{L} - L}{F}

$$

E obtém:

$$
y = \frac{q}{q - 1}x - \frac{z_F}{q - 1}
$$

que é a **equação da reta q**. Ela também mostra que a reta q sempre cruza a diagonal no ponto:

$$
x=y=z_{F}
$$

### O que é q

O $q$ mede o “estado térmico” da carga.  
Mais intuitivamente: ele mede **quanto da alimentação se comporta como líquido ao entrar no prato de alimentação**.

A professora diz que $q$ é uma medida da distância entre o estado real da carga e o equilíbrio líquido-vapor.


### Como a condição física da carga afeta a reta q



#### Líquido sub-resfriado

$$
q>1
$$
A reta $q$ tem inclinação positiva maior que 1.  
Ela fica inclinada para a direita, mais “vertical” que uma reta de 45°.
#### Líquido saturado
$$
q=1
$$
A reta q fica **vertical**.
#### Mistura líquido + vapor

$$
0<q<1
$$
A reta q tem inclinação negativa.
#### Vapor saturado

$$
q=0
$$
A reta q fica **horizontal**.

#### Vapor superaquecido

$$
q<0
$$

A reta $q$ volta a ter inclinação positiva, mas agora diferente do caso de líquido sub-resfriado.



## Como determinar o número de estágios teóricos

Resume-se o procedimento gráfico assim:

- construir o diagrama de equilíbrio $xy$ e a diagonal $y=x$;
- marcar as composições conhecidas;
- traçar a reta $q$;
- determinar $RR_{min}$​;
- determinar $RR_{op}$​;
- traçar a R.O.S.A.;
- traçar a R.O.S.E.;
- marcar os estágios;
- determinar a localização ótima da alimentação.


## Roteiro prático 


O enunciado te dá algo como:

- mistura binária;
- $xD$​;
- $xB$​;
- condição térmica da carga ou $q$;
- pressão e dados de equilíbrio;
- razão de refluxo $RR$ ou relação com $RR_{min}$ ​.

E pede:

- número de estágios teóricos;
- posição da alimentação;
- às vezes $RR_{min}$ ​.


### Passo 1 — Construir a curva de equilíbrio

Você precisa de uma forma de relacionar $x$ e $y$:

- por tabela experimental $xy$;
- ou por volatilidade relativa constante:

$$
y = \frac{\alpha x}{1 + x(\alpha - 1)}
$$


### Passo 2 — Desenhar a diagonal $y=x$


### Passo 3 — Marcar $xD,xB, zF$
- $xD$​: composição do topo.
- $xB$​: composição do fundo.
- $zF$​: composição da alimentação.

### Passo 4 — Determinar e desenhar a reta $q$

Se a condição física da carga for dada diretamente, você identifica o $q$.

$$
y = \frac{q}{q - 1}x - \frac{z_F}{q - 1}
$$


### Passo 5 — Determinar $RR_{min}$

Conceitualmente:

- em $RR_{min}$​ ocorre o **pinch**;
- nesse ponto, a coluna teria infinitos estágios:

$$
RR_{mín} \Rightarrow N = \infty
$$
#### Intuição física do pinch

No pinch, a reta de operação e a curva de equilíbrio quase “encostam” de modo que o degrau gráfico praticamente não avança. Por isso seriam necessários infinitos degraus.

#### Como fazer graficamente

Você acha o ponto crítico associado à alimentação e traça a reta da seção de topo passando por $xD$​ e pelo ponto de pinch. Daí tira a inclinação e obtém $RR_{min}$​

### Passo 6 — Escolher a razão de refluxo de operação $RR_{op}$

Os slides mostram:

$$
RR_{op} = 1,3 \text{ a } 1,5 , RR_{mín}
$$
### Passo 7 — Traçar a R.O.S.A.

Com $xD$​ e $RR$:


$$
y = \frac{RR}{RR + 1}x + \frac{x_D}{RR + 1}
$$

### Passo 8 — Traçar a R.O.S.E.

Ela passa:

- pela interseção entre a reta q e a R.O.S.A.;
- e pelo ponto $(xB,xB)$.

Esse é o jeito gráfico mais prático de construí-la.

### Passo 9 — Fazer os degraus

Agora vem a parte famosa do método.

Você começa em $xD$​ e faz:

- horizontal até a curva de equilíbrio;
- vertical até a reta de operação;
- horizontal até a curva;
- vertical até a reta;

e repete.

#### Acima da alimentação

Usa a **R.O.S.A.**

#### Abaixo da alimentação

Usa a **R.O.S.E.**

A mudança de reta acontece quando você cruza a reta $q$, isto é, no estágio de alimentação ótimo.

# References

[[Vaso Flash]]