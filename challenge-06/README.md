# Desafio da semana #5

```js
/*
Vamos falar um pouco sobre "Futebol". Escolha um campeonato estadual qualquer
para começar o desafio.
Declare uma variável chamada `championship` que receberá o nome do campeonato,
e imprima o nome desse campeonato no console.
*/

var championship = "Pernambucano";
console.log(champioship);

/*
Declare uma variável chamada `teams`, que receberá um array com 5 elementos.
Os elementos serão nomes de times do campeonato escolhido, e os nomes devem
estar na ordem em que eles aparecem na tabela no momento da solução desse
desafio.
*/

var teams = ['Sport', 'Santa Cruz', 'Náutico', 'Salgueiro', 'Central'];

console.log( 'Times que estão participando do campeonato:', teams );

/*
Crie uma função chamada `showTeamPosition` com as seguintes características:
    - A função deve receber um número por parâmetro;
    - A função deve retornar a frase:
    "O time que está em [POSIÇÃO]º lugar é o [NOME DO TIME].";
    - Onde [POSIÇÃO] é o valor passado por parâmetro e [NOME DO TIME] é o time
    que está nessa posição no array criado acima com os nomes dos times.
    --------------
    Dica: lembre-se que arrays começam no índice zero, então a posição passada
    deve ser sempre um número a mais que o índice do array ;)
    --------------
    - A função só deve retornar a frase acima somente se o time estiver entre
    os 5 primeiros.
    - Se não houver time para a posição passada, deve retornar a mensagem:
    "Não temos a informação do time que está nessa posição."
*/

var championship = "Pernambucano";
var teams = ['Sport', 'Santa Cruz', 'Náutico', 'Salgueiro', 'Central'];


function showTeamPosition(position) {
   if((position <= 5) && (position > 0)) {
    return 'O time que está em '+ (position) + 'º lugar é o '+ (teams[position - 1]) +'.';
   }
   return 'Não temos a informação do time que está nessa posição.'
}

/*
Escolha 4 times do campeonato selecionado e mostre a posição dele, usando a
função acima. Entre esses 4, adicione 1 que não esteja entre os 5 primeiros.
*/

console.log(showTeamPosition(1))
console.log(showTeamPosition(2))
console.log(showTeamPosition(3))
console.log(showTeamPosition(4))
console.log(showTeamPosition(6))
/*
O time que está em 1º lugar é o Sport.
O time que está em 2º lugar é o Santa Cruz.
O time que está em 3º lugar é o Náutico.
O time que está em 4º lugar é o Salgueiro.
Não temos a informação do time que está nessa posição.
*/

/*
Mostre os números de 20 a 30 no console (inclusive o 30), usando a estrutura de
repetição "while".
*/

var count = 20;
while(count <=30) {
    console.log(count);
    count++
}

/*
Crie uma função chamada `convertToHex`, com as seguintes características:
    - A função recebe uma cor por parâmetro, do tipo string. Exemplo: "red";
    - Escolha 5 cores que serão convertidas do nome da cor para o seu
    equivalente hexadecimal (pode ser qualquer tom);
    - Usando a estrutura switch, verifique se a cor passada por parâmetro é
    algum hexa escolhido. Se for, retorne a frase:
    "O hexadecimal para a cor [COR] é [HEXADECIMAL].";
    - Se a cor passada por parâmetro não estiver entre as selecionadas, mostre
    a frase:
    "Não temos o equivalente hexadecimal para [COR]."
*/

/*
Crie uma função chamada `convertToHex`, com as seguintes características:
    - A função recebe uma cor por parâmetro, do tipo string. Exemplo: "red";
    - Escolha 5 cores que serão convertidas do nome da cor para o seu
    equivalente hexadecimal (pode ser qualquer tom);
    - Usando a estrutura switch, verifique se a cor passada por parâmetro é
    algum hexa escolhido. Se for, retorne a frase:
    "O hexadecimal para a cor [COR] é [HEXADECIMAL].";
    - Se a cor passada por parâmetro não estiver entre as selecionadas, mostre
    a frase:
    "Não temos o equivalente hexadecimal para [COR]."
*/

function convertToHex(cor) {
    var red = '#FF0000';
    var black = '#000000';
    var yellow = '#FFFF00';
    var white = '#FFFFFF';
    var blue = '#0000FF';
    var returnMsg = 'O hexadecimal para a cor ' + cor + ' é ';

    switch (cor) {
        case 'red':
            console.log(returnMsg + red);
            break;
        case 'black':
            console.log(returnMsg + black);
            break;
        case 'yellow':
            console.log(returnMsg + yellow);
            break;
        case 'white':
            console.log(returnMsg + white);
            break;
        case 'blue': 
            console.log(returnMsg + blue);
            break;
            default:
                console.log('Não temos o equivalente hexadecimal para a ' + cor);
    }
}

/*
Tente mostrar o hexadecimal de 8 cores diferentes usando a função criada acima.
*/
convertToHex('red');
convertToHex('blue');
convertToHex('white');
convertToHex('yellow');
convertToHex('black');
convertToHex('pink');
convertToHex('DarkRed');
convertToHex('Orange');

/*
O hexadecimal para a cor blue é #0000FF
O hexadecimal para a cor white é #FFFFFF
O hexadecimal para a cor yellow é #FFFF00
O hexadecimal para a cor black é #000000
Não temos o equivalente hexadecimal para a pink
Não temos o equivalente hexadecimal para a DarkRed
Não temos o equivalente hexadecimal para a Orange

*/