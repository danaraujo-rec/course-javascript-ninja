# Desafio da semana #7
```js
/*
Crie um array com 5 items (tipos variados).
*/
var myArray = ['José', 29, {altura: 1.84}, null, function soma(){}];

/*
Crie uma função chamada `addItem`, que irá adicionar itens no array criado.
A função deverá retornar o array atualizado.
*/

function addArray(valor) {
    myArray.push(valor);
    return myArray;
}

/*
Adicione um novo array ao array criado no início do desafio, com ao menos 3
itens de tipos diferentes, mostrando o resultado no console.
*/

(addArray([25, {corDosOlhos: 'castanhos'}, null]));

/*
Mostre no console o segundo elemento desse último array, criado acima, com a
frase:
"O segundo elemento do segundo array é [ELEMENTO]."
*/

console.log('O segundo elemento do segundo array é ' + myArray[5][1].corDosOlhos + '.')

/*
Mostre no console quantos itens tem o primeiro array criado, com a frase:
"O primeiro array tem [QUANTIDADE DE ITENS] itens."
*/

console.log("O primeiro array tem " + myArray.length + " itens.")

/*
Agora mostre no console quantos itens tem o segundo array criado, com a frase:
"O segundo array tem [QUANTIDADE DE ITENS] itens."
*/

console.log("O segundo array tem " + myArray[5].length + " itens.");

/*
Utilizando a estrutura de repetição `while`, mostre no console todos os números
pares entre 10 e 20, inclusive esses 2.
*/
console.log( 'Números pares entre 10 e 20:' );

var count = 10;
while (count <= 20) {
    count % 2 === 0 ? console.log(count) : "";
    count++;
}

/*
Na mesma ideia do exercício acima: mostre agora os números ímpares.
*/
console.log( 'Números ímpares entre 10 e 20:' );

var count = 10;
while (count <= 20) {
    count % 2 === 1 ? console.log(count) : "";
    count++;
}

/*
Repita os mesmos exercícios feitos acima, mas agora usando o loop "for".
Só vamos mudar o range:
- No primeiro "for", mostre os números pares entre 100 e 120, inclusive eles;
- No segundo "for", mostre os números ímpares entre 111 e 125, inclusive eles.
*/
//criei um for já implementando os dois para, assim, diminuir a linha de código
console.log( 'Números pares entre 100 e 120:' );

for(var count = 100; count <= 120; count++) {
    count % 2 === 1 ? console.log('números ímpares: ' + count) : console.log('números pares: ' + count)
}

console.log( 'Números ímpares entre 111 e 125:' );

for(var count = 100; count <= 120; count++) {
    count % 2 === 1 ? console.log('números ímpares: ' + count) : console.log('números pares: ' + count)
}