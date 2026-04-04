
2026-04-01 21:38

Status: #baby #portuguse 

Tags: [[Faculdade]] [[Operacoes Unitarias II]]


# Exemplo 1 - Topico 3


Considere um flash de equilíbrio **adiabático**.

(a) Determine o número de **variáveis**.
(b) Descreva todas as **equações independentes** que relacionam as variáveis.
(c) Determine o **número de equações**.
(d) Determine o **número de graus de liberdade** e quais seriam as **especificações preferenciais**?
(e) Para um flash com **carga térmica** qual o **grau de liberdade**?

---

### Descrição do Diagrama do Processo

O diagrama ilustra um sistema de separação tipo flash (ou vaso de flash). Ele é composto pelos seguintes elementos:

* **Alimentação ($F$):** Uma corrente de entrada, denotada pela letra $F$, que flui horizontalmente da esquerda para a direita.
* **Válvula:** A corrente de alimentação passa por uma válvula de expansão (representada pelo símbolo clássico de dois triângulos unidos pelos vértices, semelhante a uma gravata borboleta) antes de entrar no vaso.
* **Vaso Separador:** Um tanque vertical de cantos arredondados onde ocorre a separação de fases. A alimentação entra pela lateral esquerda deste vaso.
* **Corrente de Topo ($V$):** Uma corrente que sai pela parte superior do vaso e segue para a direita, denotada pela letra $V$, representando a fase vapor.
* **Corrente de Fundo ($L$):** Uma corrente que sai pela parte inferior do vaso e segue para a direita, denotada pela letra $L$, representando a fase líquida.

# Resolucao

Claro. Vou responder como uma resolução de exercício, mas explicando o raciocínio inteiro por trás da contagem.

Antes de começar, um ponto importante: aqui não estamos usando só a **regra de fases de Gibbs** para o estado termodinâmico. Estamos fazendo a **análise de graus de liberdade da unidade de processo**, isto é, contando variáveis de correntes e restrições de balanço/equilíbrio pela metodologia (N_i = N_v - N_r). Essa é exatamente a abordagem usada nos slides de **Graus de Liberdade**. (Arquivo: _EQE482-Topico03.pdf_, slides 29–30)

---

## Reescrevendo o enunciado de forma organizada

Temos um **flash de equilíbrio adiabático**:

- entra uma corrente de alimentação (F),
    
- sai uma corrente de vapor (V),
    
- sai uma corrente de líquido (L),
    
- no vaso ocorre separação em **equilíbrio líquido-vapor**.
    

Pede-se:

1. número de variáveis;
    
2. equações independentes;
    
3. número de equações;
    
4. graus de liberdade e especificações preferenciais;
    
5. para o caso com **carga térmica (Q)**, qual o grau de liberdade.
    

Esse conteúdo aparece diretamente no exercício dos slides de graus de liberdade e também nos slides de flash. (Arquivo: _EQE482-Topico03.pdf_, slides 46–50) e (Arquivo: _EQE482-Topico04.pdf_, slides 3–4 e 13–15)

---

### 1) Contexto físico: o que é um flash?

Um vaso flash é o equipamento mais simples de separação por equilíbrio de fases. A ideia física é:

- a alimentação entra,
    
- dentro do vaso uma parte fica como **líquido**,
    
- outra parte fica como **vapor**,
    
- as duas fases saem em equilíbrio entre si.
    

Nos slides, isso é descrito como um equipamento de separação por equilíbrio de fases, em que a separação pode ocorrer por calor ou por variação de pressão. (Arquivo: _EQE482-Topico04.pdf_, slide 2)

Quando o estágio está em equilíbrio:

[  
T_V = T_L  
]  
[  
P_V = P_L  
]  
[  
y_i = K_i x_i  
]

ou seja, vapor e líquido saem à mesma temperatura, à mesma pressão e com composições relacionadas pelo equilíbrio. (Arquivo: _EQE482-Topico04.pdf_, slide 4)

---

### 2) Dados, incógnitas e objetivo

#### Dados conceituais do problema

Temos uma mistura com (C) componentes.

#### Incógnitas

Queremos contar quantas variáveis existem na unidade e quantas equações independentes as relacionam.

#### Objetivo

Determinar o grau de liberdade da unidade flash.

---

## (a) Número de variáveis

#### Ideia de primeiros princípios

Para caracterizar uma **corrente material**, precisamos conhecer:

- vazão molar;
    
- temperatura;
    
- pressão;
    
- composição.
    

Isso está explicitamente nos slides de graus de liberdade. (Arquivo: _EQE482-Topico03.pdf_, slides 29–33)

Para uma corrente com (C) componentes:

- 1 variável de vazão;
    
- 1 variável de temperatura;
    
- 1 variável de pressão;
    
- (C-1) frações molares independentes.
    

Por que (C-1) e não (C)?  
Porque as frações molares somam 1:

[  
\sum_{i=1}^{C} z_i = 1  
]

então, se você conhece (C-1) delas, a última fica automaticamente determinada.

Logo, uma corrente material tem:

[  
1+1+1+(C-1)=C+2  
]

variáveis independentes.

No flash adiabático há **3 correntes**:

- alimentação (F),
    
- vapor (V),
    
- líquido (L).
    

Então:

[  
N_v^U = 3(C+2)=3C+6  
]

Esse é exatamente o resultado dos slides. (Arquivo: _EQE482-Topico03.pdf_, slide 47)

#### Resposta do item (a)

[  
\boxed{N_v^U = 3C + 6}  
]

---

## (b) Equações independentes que relacionam as variáveis

Agora vamos listar, com cuidado, todas as restrições independentes.

## 1. Balanço global de massa

A massa total que entra deve ser igual à massa total que sai:

[  
F = L + V  
]

Essa equação aparece diretamente nos slides de flash. (Arquivo: _EQE482-Topico04.pdf_, slide 3)

Número de equações: **1**

---

## 2. Balanços de massa por componente

Para cada componente (i):

[  
F z_i = L x_i + V y_i  
]

Isso também aparece diretamente nos slides. (Arquivo: _EQE482-Topico04.pdf_, slide 3)

Agora vem um detalhe importante: embora existam (C) componentes, só **(C-1)** desses balanços são independentes.

Por quê?

Porque, se você somar todos os balanços por componente, obtém o balanço global. Então um deles fica redundante.

Número de equações independentes: **(C-1)**

---

## 3. Balanço de energia

Como o flash é **adiabático**, não há troca de calor com o meio:

[  
Q=0  
]

Então o balanço de energia da unidade fica, em forma conceitual:

[  
F H_F = L H_L + V H_V  
]

Nos slides, para o caso com carga térmica, aparece:

[  
F H_F + Q = L H_L + V H_V  
]

então, no caso adiabático, basta tomar (Q=0). (Arquivo: _EQE482-Topico04.pdf_, slide 13)

Número de equações: **1**

---

## 4. Relações de equilíbrio

Para cada componente (i), no equilíbrio líquido-vapor:

[  
y_i = K_i x_i  
]

ou equivalentemente:

[  
K_i = \frac{y_i}{x_i}  
]

Isso está nos slides do flash. (Arquivo: _EQE482-Topico04.pdf_, slide 4)

Como isso vale para cada componente, temos:

Número de equações: **(C)**

---

## 5. Restrições inerentes do estágio de equilíbrio

Como vapor e líquido saem do mesmo estágio em equilíbrio:

[  
T_V = T_L  
]

[  
P_V = P_L  
]

Essas igualdades aparecem explicitamente no slide do flash. (Arquivo: _EQE482-Topico04.pdf_, slide 4)

Número de equações: **2**

---

## Observação importante sobre soma de frações molares

Você pode se perguntar: “não faltam as equações (\sum x_i=1), (\sum y_i=1), (\sum z_i=1)?”

Aqui a resposta é: **não entram como equações adicionais independentes**, porque a contagem de variáveis já foi feita usando apenas (C-1) composições independentes por corrente. Então essa restrição já foi embutida na própria definição do número de variáveis.

---

## Resposta do item (b)

As equações independentes são:

[  
F=L+V  
]

[  
F z_i = L x_i + V y_i \qquad (C-1 \text{ independentes})  
]

[  
F H_F = L H_L + V H_V  
]

[  
y_i = K_i x_i \qquad (i=1,\dots,C)  
]

[  
T_V=T_L  
]

[  
P_V=P_L  
]

Isso coincide exatamente com a lista dos slides. (Arquivo: _EQE482-Topico03.pdf_, slide 48)

---

# (c) Número de equações

Agora basta somar:

- balanço global de massa: (1)
    
- balanços por componente: (C-1)
    
- balanço de energia: (1)
    
- relações de equilíbrio: (C)
    
- igualdade de (T) e (P): (2)
    

Logo:

[  
N_r^U = 1 + (C-1) + 1 + C + 2  
]

[  
N_r^U = 2C + 3  
]

Esse é exatamente o resultado dado no slide do exercício. (Arquivo: _EQE482-Topico03.pdf_, slide 49)

## Resposta do item (c)

[  
\boxed{N_r^U = 2C + 3}  
]

---

# (d) Número de graus de liberdade e especificações preferenciais

## Cálculo do grau de liberdade

Pela metodologia dos slides:

[  
N_i^U = N_v^U - N_r^U  
]

Substituindo:

[  
N_i^U = (3C+6) - (2C+3)  
]

[  
N_i^U = C+3  
]

Esse é exatamente o resultado mostrado no exercício. (Arquivo: _EQE482-Topico03.pdf_, slide 50)

## Resposta do item (d): grau de liberdade da unidade

[  
\boxed{N_i^U = C + 3}  
]

---

## Mas o que isso significa fisicamente?

Significa que, para o problema da unidade ficar completamente especificado, precisamos fixar (C+3) variáveis independentes.

Agora vem a parte mais importante: **quais especificações são preferenciais?**

### Passo 1: especificar completamente a alimentação

Uma corrente material precisa de (C+2) variáveis. Então, para a alimentação, normalmente especificamos:

- (F)
    
- (z_1, z_2, \dots, z_{C-1})
    
- (T_F)
    
- (P_F)
    

Total:

[  
C+2  
]

### Passo 2: falta apenas 1 especificação

Como o grau de liberdade total é (C+3), depois de especificar a alimentação ainda falta:

[  
(C+3) - (C+2) = 1  
]

Ou seja, no flash **adiabático**, depois de a carga estar totalmente definida, precisamos especificar **mais uma variável**.

Essa variável será, tipicamente:

- **a pressão do vaso** (P_V=P_L), ou
    
- **a temperatura de equilíbrio** (T_V=T_L)
    

Nos slides do exercício aparece exatamente essa separação:

- grau de liberdade total (= C+3),
    
- especificação da carga (= C+2),
    
- sobra (1),  
    com destaque para (P_V=P_L) e (T_V=T_L). (Arquivo: _EQE482-Topico03.pdf_, slide 50)
    

---

## Quais são as especificações preferenciais?

### Preferência prática 1: especificar a alimentação inteira

[  
F,; z_i,; T_F,; P_F  
]

### Preferência prática 2: especificar a pressão do flash

[  
P_V = P_L  
]

Essa costuma ser a escolha mais natural quando há uma **válvula de expansão** antes do vaso, porque o flash frequentemente é causado justamente pela queda de pressão. Isso aparece inclusive no exemplo de flash adiabático dos slides, em que a alimentação está a uma pressão e a saída do vaso está em outra pressão especificada. (Arquivo: _EQE482-Topico04.pdf_, slides 16–17)

### Alternativa

Também pode ser especificada a temperatura de equilíbrio do vaso:

[  
T_V = T_L  
]

mas, em um flash adiabático com válvula, a pressão costuma ser mais natural como variável de processo.

---

## Resposta completa do item (d)

- Grau de liberdade da unidade:
    

[  
\boxed{N_i^U = C+3}  
]

- Se a alimentação já estiver completamente especificada ((C+2)), sobra:
    

[  
\boxed{1}  
]

- Especificações preferenciais:
    
    - especificar completamente a alimentação (\big(F, z_i, T_F, P_F\big));
        
    - e especificar **uma** variável adicional do vaso, preferencialmente a **pressão do flash** ((P_V=P_L)), ou alternativamente a **temperatura** ((T_V=T_L)).
        

---

# (e) Para um flash com carga térmica, qual o grau de liberdade?

Agora o sistema deixa de ser adiabático, então aparece uma nova variável de processo:

[  
Q  
]

Fisicamente, isso aumenta o número de variáveis em 1, mas **não cria uma nova equação independente**, porque o balanço de energia continua sendo um só.

Por isso, o grau de liberdade aumenta em 1 em relação ao caso adiabático.

Nos slides de flash com carga térmica aparece diretamente:

[  
N_i^U = C+4  
]

e, pelo teorema de Duhem, uma vez conhecidas as quantidades da carga ((C+2)), restam apenas **2 variáveis** para descrever completamente o sistema. (Arquivo: _EQE482-Topico04.pdf_, slide 13)

Também aparecem exemplos de pares de especificação possíveis:

- ((P,T))
    
- ((P,\beta))
    
- ((T,\beta))
    
- ((Q,P))
    

(Arquivo: _EQE482-Topico04.pdf_, slides 14–15)

## Então, qual é a resposta?

### Grau de liberdade da unidade completa:

[  
\boxed{N_i^U = C+4}  
]

### Grau de liberdade remanescente, se a alimentação já estiver especificada:

[  
\boxed{2}  
]

Essa é a forma mais útil na prática de cálculo.

---

# Resposta final, organizada

## (a) Número de variáveis

[  
\boxed{N_v^U = 3C+6}  
]

## (b) Equações independentes

- 1 balanço global:  
    [  
    F=L+V  
    ]
    
- (C-1) balanços de componente:  
    [  
    Fz_i=Lx_i+Vy_i  
    ]
    
- 1 balanço de energia (adiabático):  
    [  
    FH_F=LH_L+VH_V  
    ]
    
- (C) relações de equilíbrio:  
    [  
    y_i=K_i x_i  
    ]
    
- 2 restrições inerentes:  
    [  
    T_V=T_L,\qquad P_V=P_L  
    ]
    

## (c) Número de equações

[  
\boxed{N_r^U = 2C+3}  
]

## (d) Graus de liberdade e especificações preferenciais

[  
\boxed{N_i^U = N_v^U-N_r^U = C+3}  
]

Se a alimentação estiver totalmente especificada ((C+2)), sobra:

[  
\boxed{1}  
]

Especificações preferenciais:

- especificar a alimentação completa:  
    [  
    F,; z_i,; T_F,; P_F  
    ]
    
- e mais uma variável do flash, preferencialmente:  
    [  
    \boxed{P_V=P_L}  
    ]  
    ou, alternativamente,  
    [  
    \boxed{T_V=T_L}  
    ]
    

## (e) Flash com carga térmica

- grau de liberdade da unidade:  
    [  
    \boxed{N_i^U = C+4}  
    ]
    
- se a alimentação já estiver especificada:  
    [  
    \boxed{2}  
    ]
    

---

# Mini-resumo do método

- contar variáveis de cada corrente como (C+2);
    
- multiplicar pelo número de correntes;
    
- contar as restrições:
    
    - balanço global,
        
    - balanços por componente,
        
    - balanço de energia,
        
    - equilíbrio,
        
    - igualdades de (T) e (P);
        
- aplicar:  
    [  
    N_i = N_v - N_r  
    ]
    

---

# O que é essencial guardar

- **flash adiabático**:  
    [  
    N_v^U=3C+6,\qquad N_r^U=2C+3,\qquad N_i^U=C+3  
    ]
    
- se a **alimentação já estiver especificada**, sobra **1 variável**;
    
- essa variável normalmente é a **pressão do vaso**;
    
- com **carga térmica**, o grau de liberdade aumenta em 1:  
    [  
    N_i^U=C+4  
    ]  
    e, com a carga fixa, sobram **2 variáveis**.
    

Quer que eu agora transforme essa resolução em um formato de **resposta de prova**, mais curta e direta, para você decorar?

# References
