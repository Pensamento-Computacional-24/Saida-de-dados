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

document.write(`A soma de A + B é ${A+B}`);

document.write(`O valor de A é ${A} e o valor de B é ${B}`);
```

Observando, para toda variável é necessário encapsulá-la (colocar dentro) na sintaxe ```${}```, para que esta funcione adequadamente. Outro fator que conta bastante é a clareza do código.

Para além da utilização do ```document.write()``` temos o ```alert()```, que recebe a mesma esturura de texto, diferenciando apenas na saída vísual em tela. Um em texto o outro em caixa de alerta.


## Quebra de Linha

A quebra de linha pode ser feita de diversas formas, mas tudo depende de qual tipo de saída você está utilizando.

Por meio do ```document.write()``` a quebra de linha acontece pela tag ```<br>``` proveniente da linguagem de marcação HTML. Ex:

```
document.write("Primeira linha <br> Segunda linha <br> Terceira linha");
```

## Conversões

Quando lidamos com tipos de dados existem três tipos básicos: Strings (texto), Int (números) e Boolean (Verdadeiro/Falso). 
Entre número e texto é bem simples converter, podemos utilizar funções como ferramenta, como o exemplo abaixo:

```
let CPFTexto = "12345678998"; // Sabedo que este número seria facilmente o CPF 123.456.789-98, podemos converte-lo para número
let CPFNumero = parseInt(CPFTexto); // Nesse caso, a função parseInt() recebe o texto entre os parenteses
```

Assim como a conversão de texto em número, também existe a possibilidade de converter números em texto.

```
let CPFNumero = 12345678998; // Seguindo o mesmo exemplo acima
let CPFTexto = CPFNumero.toString(); // Nesse caso, a variável invoca a função toString() através do ponto "."
```

Outra possibilidade é transitar entre grupos de números, ou seja, transformar um inteiro em decimal e vice versa.

```
let decimal1 = 575.53842496565;
let inteiro1 = parseInt(decimal1); // inteiro1 valerá 575

let inteiro2 = 120;
let decimal2 = praseFloat(inteiro2).toFixed(3); // decimal2 valerá 120.000
```

Em ambas as funções ```parseInt()``` e ```parseFloat()``` um valor deve ser passado como parâmetro entre os parenteses, seja ele do tipo texto ou número.
Quando a conversão ocorre de inteiro para decimal, que é incomum, é previsto que as casas decimais sejam "0" e dessa forma podemos utilizar a função ```toFixed()``` para definir quantas terão. O valor "3" entre parênteses indica quantas casas após a vírgula existirão.

