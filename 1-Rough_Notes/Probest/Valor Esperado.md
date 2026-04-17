
2026-04-15 20:45

Status: #baby #portuguse 

Tags: [[Faculdade]] [[Probabilidade e Estatistica]] [[Bloco 2 - Variáveis aleatórias discretas e distribuições clássicas]]



# Valor Esperado

Os slides definem o **valor esperado** de uma variável discreta por:
$$
E(X) = \sum_{x \in \Omega_X} x P(X = x) = \sum_{x \in \Omega_X} x p_X(x)
$$
e dizem que ele é uma medida de centralidade que depende apenas da distribuição da variável

## O que isso quer dizer?

O valor esperado é o “centro” probabilístico da variável.

Não quer dizer necessariamente um valor que vai aparecer numa realização específica.  
Ele é mais como uma **média de longo prazo**.

### Exemplo intuitivo

Se você repete um experimento muitas vezes, o valor médio observado tende a ficar perto do valor esperado.

### Caso Bernoulli

caso $X \sim Ber(p)$ entao

$$
E(X) = p
$$

Isso faz muito sentido:

- se 1 significa sucesso;
- e 0 significa fracasso;

então a média de muitas repetições é justamente a fração de sucessos, isto é, $p$.


### Caso Binomial

Os slides mostram:

$$
E(X)=np
$$


Interpretação:

- se você faz nnn tentativas;
- e cada uma tem chance $p$ de sucesso;

então o número médio de sucessos esperado é $np$.

### Caso Poisson

Os slides mostram:

$$
E(X)=\lambda
$$

Ou seja: no modelo Poisson, o parâmetro $\lambda$ já é a média.






# References
