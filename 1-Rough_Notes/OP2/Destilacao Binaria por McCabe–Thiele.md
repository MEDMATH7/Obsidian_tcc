
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


## Caso 1 - Duas cargas e nenhuma retirada lateral

Ideia:

$$
\begin{align}

F_1 = 500 \text{ mol/h}, \quad z_{F1} = 0,6, \quad \beta_1 = 0,7  \\


F_2 = 1000 \text{ mol/h}, \quad z_{F2} = 0,3, \quad \beta_2 = 0  \\


y_D = 0,95, \quad x_B = 0,05, \quad \alpha = 2,5, \quad RR_{op} = 2RR_{mín}

\end{align}
$$




### O que muda quando há duas cargas?


No caso clássico de McCabe–Thiele com uma única carga, você tem:

- uma seção de topo;
- uma seção de fundo;
- uma reta $q$.

Quando existem **duas cargas** e **nenhuma retirada lateral**, a coluna passa a ter:

- **seção de topo**;
- **seção intermediária**;
- **seção de fundo**.

Ou seja, agora existem **3 seções**. Isso está exatamente de acordo com os slides: uma seção de topo fica acima da primeira perturbação, uma seção intermediária fica entre duas perturbações, e a seção de fundo fica abaixo da última perturbação.


### A primeira coisa que você deve fazer: ordenar as cargas

Antes de qualquer conta, você precisa saber **qual carga está mais acima** e **qual está mais abaixo** na coluna.

Vou adotar a convenção:

- $F_{1}$​: carga mais alta na coluna;
- $F_{2}$​: carga mais baixa na coluna.

Então a coluna fica assim, de cima para baixo:

- topo / condensador
- seção de topo
- **carga $F_{1}$​**
- seção intermediária
- **carga $F_{2}$​**
- seção de fundo
- refervedor / fundo

Se o enunciado não disser explicitamente a ordem, você precisa defini-la a partir do desenho.

### Quais são as informações típicas do problema?

Num problema gráfico com duas cargas, normalmente você terá algo como:

- composição do produto de topo;
- composição do produto de fundo;
- composição de cada carga;
- estado térmico de cada carga, ou $q_{1}$​ e $q_{2}$​;
- razão de refluxo de operação​;
- curva de equilíbrio $xy$, ou volatilidade relativa constante $\alpha$.

No exercício dos slides, a curva de equilíbrio é dada por:

$$


y = \frac{\alpha x}{1 + x(\alpha - 1)}


$$

### O diagrama gráfico continua o mesmo em essência


Mesmo com duas cargas, o plano gráfico continua sendo:

- eixo $x$: composição do mais volátil no líquido;
- eixo $y$: composição do mais volátil no vapor;
- curva de equilíbrio;
- diagonal $y=x$.

Até aqui, nada muda. O que muda são:

- agora há **duas retas $q$**;
- agora há **três retas de operação**.

### Quais retas aparecem agora?

#### Reta de operação da seção de topo — R.O.S.A.


$$


y = \frac{RR}{RR + 1}x + \frac{x_D}{RR + 1}


$$


#### Reta de operação da seção intermediária — R.O.S.INT.

Essa é a novidade principal.

Nos slides aparece, para a seção intermediária de uma coluna com duas cargas:

$$
y_j = \frac{\bar{L}}{\bar{V}}x_{j-1} + \frac{Dx_D - F_1z_{F1}}{\bar{V}}
$$


#### Reta de operação da seção de fundo — R.O.S.E.

Abaixo da segunda carga, você volta a ter a seção de fundo, que pode ser escrita como:

$$
y = \frac{L_2}{V_2}x - \frac{B}{V_2}x_B
$$
ou, graficamente, você pode construí-la passando por:

- o ponto de transição na segunda carga;
- e o ponto $(xB,xB)$, no caso usual de fundo líquido saturado.

Nas suas notas você já tinha a ideia de que a R.O.S.E. passa pelo ponto$(xB,xB)$.

### As duas retas q

Como existem duas cargas, agora existem:

- reta $q_{1}$​, associada a $F_{1}$​;
- reta $q_{2}$​, associada a $F_{2}$​.

Cada uma é traçada com a forma:

$$
y = \frac{q}{q - 1}x - \frac{z_F}{q - 1}
$$
e cada uma passa pela diagonal no ponto:

$$
x = y = zF
$$



### Como calcular o estado térmico das duas cargas


Usa-se $\beta$ para a parte vaporizada da carga e então calcula:

$$
q = 1 - \beta
$$
Para a carga 1:

$$
\beta_1 = 0,7 \Rightarrow q_1 = 1 - 0,7 = 0,3
$$
Para a carga 2:

$$
\beta_2 = 0 \Rightarrow q_2 = 1
$$

### Resolução gráfica passo a passo


#### Passo 0 — organizar os dados

Separa-se:

$$
\begin{align}

F_1, z_{F1}, q_1  \\


F_2, z_{F2}, q_2  \\


x_D \text{ ou } y_D, \text{ dependendo do topo}  \\


x_B  \\


RR_{op}  \\


\text{curva de equilíbrio}

\end{align}
$$

#### Passo 1 — construir a curva de equilíbrio e a diagonal

Usa-se:

$$
y = \frac{\alpha x}{1 + x(\alpha - 1)}
$$

e depois a diagonal

$$
y=x
$$

#### Passo 2 — marcar as composições importantes

No gráfico marque:

$$
\begin{align}

z_{F1}  \\


z_{F2}  \\


x_B  \\


x_D \text{ ou } y_D, \text{ conforme o tipo de condensador}

\end{align}
$$

#### Passo 3 — traçar as duas retas q

##### Carga 1

$$
 q_{1} = 0.3
$$
então a reta $q_{1}$ passa por $zF_{1}$ = 0.6 e em inclinação

$$
\frac{q_1}{q_1 - 1} = \frac{0,3}{-0,7} \approx -0,43
$$

##### Carga 2

$$
q_{2} = 1
$$



Logo a reta $q_{2}$ é vertical passando por

$$
zF_{2} = 0.3
$$

### Passo 4 — determinar $RR_{min}$


Pegando as duas $RR_{min}$ e utiliza a maior.




### Passo 5 — traçar a R.O.S.A.


Usando a equação da seção de topo

$$
y = \frac{RR}{RR + 1}x + \frac{x_D}{RR + 1}
$$


### Passo 6 — obter a reta intermediária R.O.S.INT.



Pelo balanço molar na seção entre $F_{1}$ e $F_{2}$ 


$$
y = \frac{L_1}{V_1}x + \frac{Dx_D - F_1z_{F1}}{V_1}
$$

Como achar $L_{1}$ e $V_{1}$

Você parte da seção de topo:

$$
\begin{align}

L_0 = RR \cdot D  \\


V_0 = L_0 + D

\end{align}
$$


Depois cruza a primeira carga. Como essa carga possui $q_{1}$​, as vazões da seção abaixo mudam.


A ideia física é:

- a parte líquida da carga aumenta $L$;
- a parte vapor aumenta $V$.

Então:

$$
\begin{align}

L_1 = L_0 + q_1 F_1  \\


V_1 = V_0 + (1 - q_1)F_1

\end{align}
$$


Isso é coerente com a interpretação de $q$ e com o modelo de seções dos slides. A formulação geral por seções também aparece no desenvolvimento analítico.


### Passo 7 — obter a R.O.S.E.

Abaixo da segunda carga:

$$
\begin{align}

L_2 = L_1 + q_2 F_2  \\


V_2 = V_1 + (1 - q_2)F_2

\end{align}
$$

E a reta de fundo pode ser escrita como:

$$
y = \frac{L_2}{V_2}x - \frac{B}{V_2}x_B
$$

ou, graficamente, como a reta que passa por:

- o ponto de encontro com a carga 2;
- o ponto $(xB,xB)$.

### Como encontrar os pontos de troca de seção

Isso é o coração do método gráfico com duas cargas.

#### Primeiro ponto de troca

É onde a seção de topo encontra a seção intermediária.

Graficamente, isso acontece na **reta $q_{1}$​**.

Então:

- você traça a R.O.S.A.;
- traça a reta $q_{1}$​;
- a interseção dessas duas define o ponto de transição superior.

#### Segundo ponto de troca

É onde a seção intermediária encontra a seção de fundo.

Graficamente, isso acontece na **reta $q_{2}$​**.

Então:

- você traça a R.O.S.INT.;
- traça a reta $q_{2}$​;
- a interseção delas define o ponto de transição inferior.

Nos slides, a professora resume exatamente isso ao dizer que os estágios que cruzam as retas $q$ são os estágios de carga ótimos.

# References

[[Vaso Flash]]