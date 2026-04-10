
2026-04-07 23:12

Status: #baby  #portuguse 

Tags: [[Faculdade]] [[TCC]] [[Economic Control of Quality Manufactured Product]] 


# Chapter 2 - Scientific Basis for Control


O que se pode dizer sobre o comportamento futuro de um fenômeno que está sob influência de causas desconhecidas ou aleatórias?

Stewhart escreve 3 postulados.

## Postulado 1 - Nem todos os sistemas aleatórios são iguais

Existem sistemas em que o acaso é tão desorganizado, instável ou mudável, que o passado quase não ajuda a prever o futuro. E existe outros sistemas em que, embora cada evento individual seja incerto, o conjunto tenha uma regularidade estatística.

### Intuição

Um evento individual pode ser imprevisível, mas o comportamento agregado talvez seja previsível.

Como por exemplo, não sei qual será o próximo deslocamento exato de uma partícula, mas talvez o deslocamento em que tendem a se distribuir sim.
Isso quer dizer que o trabalho de um engenheiro não é sair calculando, mas sim se perguntar se o tipo de variação que estou observando pertence a um sistema que permite previsão estatística ou não?

## Postulado 2 - Existem sistemas constantes de natureza aleatórias na natureza


Existem acasos em que não é bagunça completa, isso quer dizer que certos acasos tem estabilidade estatística

### A) Lei da mortalidade

Individualmente, ninguém consegue prever com precisão:

- quem vai morrer no próximo ano,
- quando,
- por qual causa.

Mas, quando você olha **grandes grupos populacionais homogêneos**, aparece uma regularidade: a taxa média de mortes em certas faixas etárias tende a não variar muito ao longo do tempo. Então, embora o evento individual seja incerto, o conjunto mostra estabilidade. Shewhart interpreta isso como uma forma de **equilíbrio estatístico**.

### B) Movimento molecular / movimento browniano

O segundo exemplo é ainda mais forte. O movimento de partículas suspensas parece totalmente irregular quando observado ponto a ponto. A direção muda o tempo todo. Você não consegue dizer com exatidão para onde a partícula irá no próximo instante. Mas, mantendo a temperatura constante, o **tipo de movimento** permanece estatisticamente o mesmo por longos períodos.

Essa é uma ideia lindíssima do capítulo:

- a trajetória instantânea parece caótica;
- a distribuição estatística dos deslocamentos apresenta regularidade.

Ou seja:

**irregularidade local não impede regularidade global.**

#### A equação que nasce daí

Com base nesses exemplos, Shewhart propõe que existem fenômenos controlados por sistemas de causas aleatórias tais que a probabilidade de uma característica $X$ cair entre $X\text{ e }X+dX$ pode ser descrita como:

$$
dy = f(X, x_1, x_2, \dots, x_m) dX
$$


Onde:

$$
\begin{align}
X = \text{característica medida;} \\

dy = \text{probabilidade associada ao pequeno intervalo;} \\

f(\cdot) = \text{função que descreve a distribuição;} \\

x_1, x_2, \dots, x_m = \text{parâmetros que caracterizam essa distribuição.}
\end{align}
$$


##### Significado físico dessa equação

Ela não te diz o valor exato da próxima peça, do próximo deslocamento ou da próxima medição.

Ela diz algo mais modesto, mas muito útil:

**ela descreve como os valores tendem a se distribuir.**

E isso é exatamente o tipo de conhecimento de que o controle estatístico precisa.


## Postulado 3 - Causas atribuíveis podem ser encontradas e eliminadas


Depois de dizer que existem sistemas constantes de acaso, Shewhart faz a ponte com a indústria real.

Ele observa que, na prática, muitos processos produtivos **não começam controlados**. Existem causas de variação que não pertencem ao sistema constante. Essas causas foram chamadas por ele de **assignable causes**, isto é, causas atribuíveis, identificáveis. Aí vem o terceiro postulado: causas atribuíveis de variação podem ser encontradas e eliminadas.

Porque, sem esse postulado, o engenheiro teria de aceitar toda variação como inevitável. Com ele, a lógica muda:


1. existe uma parte da variação que é “inerente” ao sistema constante;
2. existe outra parte que vem de causas específicas;
3. essas causas específicas podem ser investigadas e removidas.


## Como saber olhando dados reais, se há causas atribuíveis atuando?

Shewhart usa o exemplo da **fração defeituosa** ao longo de meses para dois tipos de produto. A ideia é simples:

- todo mês você observa uma fração de itens defeituosos;
- essa fração varia de mês para mês;
- a pergunta é: essa variação é apenas acaso aceitável ou sinal de problema?

### A dificuldade verdadeira

Não basta olhar e dizer “variou muito”.

Porque toda variável real flutua.

Então a pergunta correta não é:

- “há variação?”

A pergunta correta é:

- **“essa variação excede o que deveríamos deixar ao acaso?”**

E aí entra a ideia de estabelecer **limites**. 

Se os pontos observados ficam em uma faixa compatível com o comportamento esperado do sistema, talvez a variação deva ser deixada ao acaso. Se saem dessa faixa, isso pode indicar causa atribuível.

# References
