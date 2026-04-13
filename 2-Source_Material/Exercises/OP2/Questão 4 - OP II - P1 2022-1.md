
2026-04-11 11:45

Status: #baby #portuguse 

Tags: [[Destilacao Binaria por McCabe–Thiele]]


# Questão 4 - OP II - P1 2022-1

## Enunciado


QUESTÃO 4 (3,5) – Uma mistura de álcool e água é separada por destilação em uma coluna com um condensador parcial e um refervedor total. Deseja-se obter um produto de topo com 99% de álcool e um subproduto com vazão de 25 kmol/h na temperatura de 73,0 °C, a partir de uma carga contendo 40% de álcool com vazão molar de 100 kmol/h e 68% de fração vaporizada. A coluna opera a 1 atm. O produto de fundo contém 4% molar de álcool e deixa a coluna como líquido saturado. A razão de refluxo externa de topo é 2,5 vezes a razão de refluxo mínima. Usando o Método de McCabe Thiele Gráfico ou Analítico de sua escolha, Responda:

(a) (0,25) Qual a principal consequência prática das aproximações do método de McCabe Thiele?
(0,10 ponto) A consequência prática das diferenças de entalpia entre as fases líquidas e vapor serem constantes dentro de uma mesma seção é que (0,15 pontos) as vazões das correntes líquida e vapor também serão constantes na seção.

(b) (0,25) Qual o perfil da volatilidade relativa da mistura álcool/água? O que podemos concluir sobre esse perfil?
(0,15 pontos) Calculou todos os alfas e identificou constante e igual a 5. (0,10 ponto) Estamos considerando que a essa mistura de álcool e água tem comportamento de mistura ideal.

(c) (0,50) Qual a razão de refluxo mínima? Explique o que aconteceria com a coluna se operássemos com esta razão de refluxo.
(0,35 pontos) Marcou a reta q, achou y_max pelo PINCH e calculou R_R,min = 1,3 (gráfico) / Verificou z_F usando y_F do chute, achou x_F usando y_F no equilíbrio e calculou R_R,min pela relação de y_F e x_F com y_D, R_R,min = 1,4 (analítico). (0,15 pontos) Se operássemos nesta razão de refluxo a coluna daria PINCH na carga, precisaria de um número de estágios infinito para separar.

UNIVERSIDADE FEDERAL DO RIO DE JANEIRO
DEPARTAMENTO DE ENGENHARIA QUÍMICA
DISCIPLINA: EQE482 - OPERAÇÕES UNITÁRIAS II
2022-1
PROFESSORA: INGRID AZEVEDO

(d) (2,00) Qual o número de estágios teóricos para esta operação? Explique seu procedimento.
Gráfico
1- ROSA
(0,5 pontos) Calculou R_R,op=2,5 R_R,min=3,26(gráfico)/3,55(analítico) achou y_op = y_D / (R_R,op + 1) e traçou a ROSA indo de x_D (equilíbrio com y_D) até y_op.
2- ROSINT
Identificou a retirada lateral
(0,15 pontos) x_S=0,5 no diagrama de T vs. xy, curva de líquido saturado a 73°C
(0,10 pontos) Retirada é normalmente líquido saturado β_s=0, q=1.
(0,20 pontos) Fez o balanço global e por componente na coluna para determinar D.
(0,30 pontos) Usou a equação do y_rosint = (Dx_D + Sx_S) / V'', sendo V'' = D(R_R,op + 1) + β_s*S
3- ROSE
(0,5 pontos) Traçou a ROSE saindo da intercessão da carga com a ROSINT até x_B na reta de 45°
4- ESTÁGIOS
(0,25 pontos) 7 estágios teóricos ((0,2 pontos) 6 pratos + (0,05 pontos) 1 condensador)

Analítico
Identificou a retirada lateral
(0,15 pontos) x_S=0,5 no diagrama de T vs. xy, curva de líquido saturado a 73°C
(0,10 pontos) Retirada é normalmente líquido saturado β_s=0, q=1.
(0,20 pontos) Fez o balanço global e por componente na coluna para determinar D.
(0,5 pontos) Análise da seção de absorção L_0, V_0 e Somatório (-Dx_D) e ponto de mudança x_i=x_S.
(0,3 pontos) Análise da seção de intermediaria L_1, V_1 e Somatório (-Dx_D - Sx_S) e ponto de mudança x_i=x_1,2 ou y_i=y_1,2.
(0,5 pontos) Análise da seção de esgotamento L_2, V_2 e Somatório (-Dx_D - Sx_S + Fz_F) e ponto de parada x_i= x_B.
Contagem dos estágios pelo procedimento de calculo no equilíbrio e depois cálculo na reta de operação correspondente a seção até o ponto de mudança.
(0,25 pontos) 7 estágios teóricos ((0,2 pontos) 6 pratos + (0,05 pontos) 1 condensador)

(e) (0,50) Qual o prato ótimo da carga e do subproduto?
Gráfico
Estágio que cruza a reta q
(0,25 pontos) Retirada no 3° contando o condensador; sem o condensador no 2° de cima para baixo. (0,25 pontos) Carga no 4° contando o condensador; sem o condensador no 3° de cima para baixo.
Analítico
Estágio em que há a mudança de seção
(0,25 pontos) Retirada no 4° contando o condensador; sem o condensador no 3° de cima para baixo. (0,25 pontos) Carga no 5° contando o condensador; sem o condensador no 4° de cima para baixo.

DICA: Caso resolva pelo método analítico chute y_F=0,5 para análise das perturbações.



### Resolução a)


# References
