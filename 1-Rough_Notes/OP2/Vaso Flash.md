
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

## Casos possíveis de Flash

### Caso A - Dado $P,T \text{ e }z_{i}$: calcular $\beta,x_{i},y_{i}$

#### Procedimento

1 - Com $P$ e $T$, calcular $K_{i}$
2- Resolver a equação de flash

$$
\sum \frac{z_i\left(1-K_i\right)}{1+\beta\left(K_i-1\right)}=0
$$

3- Calcular

$$
\begin{gathered}
x_i=\frac{z_i}{(1-\beta)+\beta K_i} \\
y_i=K_i x_i
\end{gathered}
$$


4- Se souber F, calcular:

$$
V=\beta F, \quad L=(1-\beta) F
$$


Se reconhece esse caso:

- Quando o enunciado fala: "Dada a alimentação a tal $P$ e $T$, determine as compisoções das fases"
- "Calcula a fração vaporizada"
- "Determine as vazões de vapor e líquido"

### Caso B: Pergunta sobre a preferência de fase

Se reconhece esse caso:

- "Quais componentes saem preferencialmente no topo/vapor?"
- "Quais preferem a fase líquida?"

#### Procedimento

1- Calcular $K_{i}$
2- Comparar com 1.

Se $K_{i}>1$, vai preferencialmente para vapor
Se $K_{i}<1$, vai preferencialmente para líquido

### Caso C: Pergunta sobre a condição física da carga:

Se reconhece:

- A carga é toda líquida?
- Toda vapor?
- Mistura líquido-vapor?
- Está no ponto de bolha?
- Está no ponto de orvalho?

#### Procedimento 1:

##### Ponto de bolha

$$
\sum z_i K_i = 1
$$

##### Ponto de orvalho

$$
\sum \frac{z_i}{K_i} = 1
$$

#### Procedimento 2:

Usar $f(o) \text{ e } f(1)$

Calcula-se ambos e verifica se existe raízes entre 0 e 1

### Caso D: Dado P, determinar temperatura de bolha


Funciona da seguinte maneira,

- A composição líquida é a da carga
$$
x_{i}=z_{i}
$$

- A composição do primeiro vapor vem de:
$$
y_i = K_i x_i
$$

- Deve valer:

$$
\sum z_i K_i = 1
$$


#### Procedimento

1- Dado $P$, chutar $T$.
2- Calcular $K_{i}(T,P)$
3- Testar:

$$
\sum z_i K_i = 1
$$

4- Ajustar $T$ até satisfazer.

### Caso E: Dado $T$, determinar Pressão de bolha

Mesma lógica que caso D, porém se ajusta $P$ em vez de $T$.

### Caso F: Dado $P$, determinar temperatura de orvalho

Funciona da seguinte maneira:

No ponto de orvalho

- A composição do vapor é a de carga:

$$
y_{i} = z_{i}
$$

- A composição do primeiro líquido é:

$$
x_i = \frac{y_i}{K_i}
$$

- Deve valer:

$$
\sum \frac{z_i}{K_i} = 1
$$

#### Procedimento

1- Dado $P$, chutar $T$
2- Calcular $K_{i}$
3- Testar

$$
\sum \frac{z_i}{K_i} = 1
$$

4- Ajustar $T$

### Caso G: Dado $T$, determinar pressão de orvalho

Mesma coisa que Caso F, porém ajustando $P$.

### Caso H: Flash adiabático com queda de pressão

A alimentação entra em uma condição, passa pelo flash e na saída fica a uma pressão conhecida.

- Quais componentes preferem vapor/líquido?
- Condição física
- Vazão líquida
- Composição das saídas

Roteiro:

1- Identificar que é flash adiabático
2- Alimentação costuma estar especificada: $F,z_{i},T,P$
3- A pressão do vaso é dada
4- Calcular $K_{i}$
5- Verificar a condição física usando $f(o) \text{ e } f(1)$
6- Se houver duas fases, resolver a questão de flash para $\beta$
7- Calcular $V \text{ e }L$
8- Calcular $x_{i}\text{ e }y_{i}$

### Caso I - Flash com carga térmica $Q$


Utilizando o balanço de energia

$$
FH_F + Q = LH_L + VH_V
$$

e escrevendo nos temos de $\beta$:


$$
(1 - \beta)H_L + \beta H_V - H_F - \dot{Q} = 0
$$

com $\dot{Q} = Q / F$.

Existem quatro combinações possíveis de especificação.

1- $(P,T)$
2- $(P,\beta)$
3- $(T,\beta)$
4-  $(Q,P)$

#### caso I.1: $P\text{ e }T$ conhecidos

1- Calcular $K_{I}$
2- Resolver o flash para $\beta$
3- Calcular $x_{i},y_{i}$
4- Calcular $H_{L},H_{V}$
5- Calcular $Q$ no balanço de energia



#### caso I.2: $P\text{ e }\beta$ conhecidos

1- Usar a equação de flash para calcular $T$
2- Calcular $x_{i},y_{i}$
3- Calcular $H_{L},H_{V}$
4- Calcular $Q$ no balanço de energia

#### caso I.3: $T\text{ e }\beta$ conhecidos

1- Usar a equação de flash para calcular $P$
2- Calcular $x_{i},y_{i}$
3- Calcular $H_{L},H_{V}$
4- Calcular $Q$ no balanço de energia

#### caso I.4: $Q\text{ e }P$ conhecidos

1- Estimar $T$
2- Calcular $\beta$ pela equação de flash
3- Calcular $x_{i},y_{i}$
4- Calcular $H_{L},H_{V}$
5- Usar balanço de energia para recalcular $T$
6- Comparar e iterar


## Como reconhecer o tipo de questão

### Se o enunciado dá $P,T,z_{i}$

Flash completo

$$
K_i \rightarrow \beta \rightarrow x_i, y_i \rightarrow L, V
$$

### Se o enunciado pede só se a carga vaporiza ou condensa parcialmente

Condição física da carga

$$
f(o),f(1)
$$

ou

$$
\sum z_i K_i, \quad \sum z_i / K_i
$$

### Se o enunciado fala em primeira bolha

Ponto de bolha

$$
x_i = z_i, \quad \sum z_i K_i = 1
$$

### Se o enunciado fala em primeira gota

Ponto de orvalho

$$
y_i = z_i, \quad \sum \frac{z_i}{K_i} = 1
$$

### Se o enunciado menciona $Q$

Flash com balanço de energia

$$
FH_F + Q = LH_L + VH_V
$$

## Algoritmo

### Passo 1: Ler o enunciado e classificar o problema

- É adiabático?
- Há carga térmica?
- $P$ e $T$ são conhecidos?
- Estou no ponto de bolha/orvalho?
- Querem condição física, composições ou vazões?

### Passo 2: Identificar as incógnitas
Normalmente temos:
$$
\beta, x_i, y_i, L, V, T, P, Q
$$

### Passo 3: Escolher a relação de equilíbrio

$$
y_{i}=K_{i}x_{i}
$$
Também definir como vai calcular $K_{i}$

### Passo 4: Verificar a condição física

usar
- Ponto de bolha
- Ponto de orvalho
- Ou $f(o)\text{ e }f(1)$

### Passo 5: Se houver duas fases, resolver a equação de flash

$$
\sum \frac{z_i(1 - K_i)}{1 + \beta(K_i - 1)} = 0
$$

### Passo 6: Calcular composições das fases

$$


x_i = \frac{z_i}{(1 - \beta) + \beta K_i} \quad y_i = K_i x_i

$$


### Passo 7: Calcular vazões de fase

$$
V = \beta F, \quad L = (1 - \beta)F
$$

### Passo 8: Se houver energia, fechar o balanço

$$
FH_F + Q = LH_L + VH_V
$$




































































# References
