# Saida-de-Dados

## Concatenação

Existem 3 formas de apresentar uma saída de dados no JavaScript, saída de: usuário, back-end, front-end.
Nesse momento nós estamos focando nas saídas de usuário, uma vez que nos trás resultado vísível em tela.

Um exemplo dessas é...

```
document.write("");
```

Em poucas palavras, esse comando acessa a raiz do arquivo - estrutura ```document``` - e chama uma função de escrita ```write()```. Para essa função podemos enviar algo, um texto, número ou podemos deixá-la vazia se quisermos.

Utilizar ```""``` (aspas duplas) ou ```''``` (aspas simples) é uma forma bem simples de dizer que algo será do tipo texto. Outra forma de dizer isso é utilizando ``` `` ``` (crase). A crase facilita muito a programação, veja só:

```
// Este é um exemplo de código sem crase

document.write("A soma de A + B é "+ (A+b) );
document.write('A soma de C + D é ', (C+D) );

// O parenteses entre A+B ou C+D, permite a soma de ambos.

document.write("O valor de A é ", A, ' e o valor de B é '+ B);
```

Note que ao utilizar ambas as aspas, para fazer a concatenação, ou seja, juntar texto e número, é necessário adicionar ao final das aspas o símbolo de ```+``` ou ```,```. E que, dependendo da quantidade de variáveis, pode-se tornar trabalhoso, considerando ter que abrir e fechar sempre.

Utilizar a crase nos permite poupar mais tempo durante a codificação/programação.


```
// Este é um exemplo de código com crase

document.write(`A soma de A + B é $(A+B)`);

document.write("O valor de A é $(A) e o valor de B é $(B));
```

Observando, para toda variável é necessário encapsulá-la (colocar dentro) na sintaxe ```$()```, para que esta funcione adequadamente. Outro fator que conta bastante é a clareza do código.

Para além da utilização do ```document.write()``` temos o ```alert()```, que recebe a mesma esturura de texto, diferenciando apenas na saída vísual em tela. Um em texto o outro em caixa de alerta.


## Quebra de Linha

A quebra de linha pode ser feita de diversas formas, mas tudo depende de qual tipo de saída você está utilizando.

Por meio do ```document.write()``` a quebra de linha acontece pela tag ```<br>``` proveniente da linguagem de marcação HTML. Ex:

```
document.write("Primeira linha <br> Segunda linha <br> Terceira linha");
```

Por agora é importante que vocês conheçam esse método. As outras formas vou passando com o tempo para não pressioná-los.



