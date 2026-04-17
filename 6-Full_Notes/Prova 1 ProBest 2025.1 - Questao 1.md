
2026-04-16 23:18

Status:

Tags:  [[Faculdade]] [[Probabilidade e Estatistica]]  [[Prova - ProBest]]


# Prova 1 ProBest 2025.1 - Questao 1

Q1) Uma pessoa, quando vai para o trabalho, utiliza apenas uma das três seguintes possibilidades: seu carro 30% das vezes, anda a pé 30% das vezes e anda de ônibus 40% das vezes. Ela se atrasa 3% das vezes quando pega o carro; ela se atrasa 10% das vezes quando anda a pé e ela se atrasa 7% das vezes quando pega o ônibus.

a) Qual é a probabilidade de ela se atrasar em uma ida ao trabalho?
b) Qual é a probabilidade de ela ter ido de ônibus condicionado a ela ter se atrasado?
c) Qual é a probabilidade de ela ter ido a pé condicionado a ela não ter se atrasado?

## Resposta

Vamos resolver com bastante calma.

Essa questão é de **Lei da Probabilidade Total** e **Teorema de Bayes**, exatamente o conteúdo da **Aula 2** dos slides. A definição de probabilidade condicional aparece na **Aula 1**, e a Lei da Probabilidade Total e Bayes aparecem na **Aula 2**.

## 1) Reescrevendo o enunciado de forma organizada

Uma pessoa pode ir ao trabalho de 3 maneiras:

- **Carro**: 30% das vezes
    
- **A pé**: 30% das vezes
    
- **Ônibus**: 40% das vezes
    

Probabilidades de atraso em cada caso:

- Se vai de **carro**, atrasa com probabilidade 3%
    
- Se vai **a pé**, atrasa com probabilidade 10%
    
- Se vai de **ônibus**, atrasa com probabilidade 7%
    

Queremos calcular:

a) a probabilidade total de atraso  
b) a probabilidade de ter ido de ônibus, **sabendo que atrasou**  
c) a probabilidade de ter ido a pé, **sabendo que não se atrasou**

---

## 2) Dados

Vamos definir os eventos:

- (C): ir de **carro**
    
- (P): ir **a pé**
    
- (O): ir de **ônibus**
    
- (A): **atrasar**
    

Então:

[  
P(C)=0{,}30,\quad P(P)=0{,}30,\quad P(O)=0{,}40  
]

[  
P(A|C)=0{,}03,\quad P(A|P)=0{,}10,\quad P(A|O)=0{,}07  
]

---

## 3) O que os slides usam aqui

A **Lei da Probabilidade Total** diz que, se os casos formam uma partição do espaço amostral, então

[  
P(B)=P(A_1)P(B|A_1)+\cdots+P(A_n)P(B|A_n)  
]

Isso aparece diretamente nos slides.

E a **probabilidade condicional** é definida por

[  
P(A|B)=\frac{P(A\cap B)}{P(B)}  
]

Também está nos slides.

Além disso, o **Teorema de Bayes** aparece como

[  
P(A_i|B)=\frac{P(A_i)P(B|A_i)}{P(A_1)P(B|A_1)+\cdots+P(A_n)P(B|A_n)}  
]

---

# a) Qual é a probabilidade de ela se atrasar?

Aqui queremos (P(A)).

Como a pessoa necessariamente vai **ou de carro, ou a pé, ou de ônibus**, esses três casos formam uma partição. Então aplicamos a **Lei da Probabilidade Total**:

[  
P(A)=P(C)P(A|C)+P(P)P(A|P)+P(O)P(A|O)  
]

Substituindo:

[  
P(A)=0{,}30\cdot 0{,}03+0{,}30\cdot 0{,}10+0{,}40\cdot 0{,}07  
]

Agora calculando termo a termo:

[  
0{,}30\cdot 0{,}03=0{,}009  
]

[  
0{,}30\cdot 0{,}10=0{,}030  
]

[  
0{,}40\cdot 0{,}07=0{,}028  
]

Somando:

[  
P(A)=0{,}009+0{,}030+0{,}028=0{,}067  
]

### Resposta do item (a)

[  
\boxed{P(A)=0{,}067=6{,}7%}  
]

---

# b) Qual é a probabilidade de ela ter ido de ônibus condicionado a ela ter se atrasado?

Agora queremos:

[  
P(O|A)  
]

Pela definição de probabilidade condicional, ou equivalentemente Bayes:

[  
P(O|A)=\frac{P(O\cap A)}{P(A)}  
]

Mas

[  
P(O\cap A)=P(O),P(A|O)  
]

Então:

[  
P(O|A)=\frac{P(O)P(A|O)}{P(A)}  
]

Substituindo os valores:

[  
P(O|A)=\frac{0{,}40\cdot 0{,}07}{0{,}067}  
]

Primeiro o numerador:

[  
0{,}40\cdot 0{,}07=0{,}028  
]

Então:

[  
P(O|A)=\frac{0{,}028}{0{,}067}\approx 0{,}4179  
]

### Resposta do item (b)

[  
\boxed{P(O|A)\approx 0{,}4179=41{,}79%}  
]

Interpretação: entre as vezes em que ela se atrasa, cerca de **41,8%** foram dias em que ela foi de ônibus.

---

# c) Qual é a probabilidade de ela ter ido a pé condicionado a ela não ter se atrasado?

Agora queremos:

[  
P(P|A^c)  
]

onde (A^c) significa **não se atrasar**.

Pela definição:

[  
P(P|A^c)=\frac{P(P\cap A^c)}{P(A^c)}  
]

## Passo 1: calcular (P(A^c))

Sabemos que

[  
P(A^c)=1-P(A)=1-0{,}067=0{,}933  
]

## Passo 2: calcular (P(P\cap A^c))

A probabilidade de ir a pé e **não** se atrasar é:

[  
P(P\cap A^c)=P(P),P(A^c|P)  
]

Sabemos que:

[  
P(A|P)=0{,}10  
]

Logo,

[  
P(A^c|P)=1-0{,}10=0{,}90  
]

Então:

[  
P(P\cap A^c)=0{,}30\cdot 0{,}90=0{,}27  
]

## Passo 3: montar a condicional

[  
P(P|A^c)=\frac{0{,}27}{0{,}933}\approx 0{,}2894  
]

### Resposta do item (c)

[  
\boxed{P(P|A^c)\approx 0{,}2894=28{,}94%}  
]

---

# Respostas finais

[  
\boxed{\text{a) } 6{,}7%}  
]

[  
\boxed{\text{b) } 41{,}79%}  
]

[  
\boxed{\text{c) } 28{,}94%}  
]

---

## Mini-resumo do método usado

- Definir os eventos com clareza.
    
- Usar a **Lei da Probabilidade Total** para achar a probabilidade total de atraso.
    
- Usar a fórmula de **probabilidade condicional** ou **Bayes** para os itens condicionais.
    
- Quando aparecer “não atrasou”, usar o complementar:  
    [  
    P(A^c)=1-P(A)  
    ]
    

Quer que eu também monte essa resolução em formato mais “anotação de caderno”, bem limpa para você copiar?
# References
