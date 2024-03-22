# Declaração de variáveis 
### Para se declarar uma variável, podem se usar 3 comandos diferentes, let, var, e const, cada um com suas funções
## Let
O comando let é utilizado para criar uma variável e limitar o seu escopo em um bloco ou expressão onde ela é usada
### Exemplo Let:
```javascript
    let message = "Hello world";

    message = " Dw2";

    alert(message);
```
## Var
O comando var é utlizado para criar uma variável com escopo global, sendo visível em todo o código, Var é menos utilizado por ter seus problemas de escopo, que são mais fáceis de se controlar com os outros comandos
### Exemplo var
```javascript
//declarar variavel:
var mensagem = "Dw";
var numero = 10;

console.log(mensagem);
console.log(numero);

//alterar variavel
mensagem = "Desenvolvimento web 2";
numero = 20;
console.log(mensagem);
console.log(numero);
```
## Const
 O comando const é utilizado para se criar variáveis que não podem ter seus valores alterados ou reatribuídos, sendo imutáveis, qualquer tentativa de alteração de valor vai dar um erro
 ## Exemplo erro
 ```javascript
const PI = 3.14159;
PI = 3;
```
## EXEMPLOS
```javascript
//Declarando
const nome = "Alice";
const idade = 30;

// Declarando uma variável com um objeto
const pessoa = {
    nome: "João",
    idade: 25
};

// É possível modificar um atributo da variável
pessoa.idade = 26;

//Tentando reatribuir (vai dar erro)
pessoa = { nome: "Maria", idade: 35 };

// Exibir os valores

console.log(PI);
console.log(nome);
console.log(idade);
console.log(pessoa);
```
# Escopo
### O escopo de uma variável é a que parte do código a variável se aplica, o global sendo em todo o código, enquanto o de bloco por exemplo, é limitado a uma área específica

## Escopo global
Uma variável com escopo global é uma variavel que pode ser acessada em qualquer lugar do código.
Um exemplo disso são variáveis do tipo var, que possuem escopo global podendo ser acessadas em qualquer ponto do código.
## Exemplo
``` javascript
var mensagem = "DW 2";

function funcao() {
    console.log(mensagem);
}

funcao();

console.log(mensagem);
```
A variável foi criada fora da função, mas pode ser acessada dentro ou fora dela.

## Escopo de Bloco
Uma variável com escopó de bloco é uma variável que pode ser isolada em um bloco, e não pode ser acessada de fora desse bloco, como por exemplo as variáveis de tipo let.

## Exemplo
```javascript
function funcao() {
    let mensagem = "Hello world"; 

    if (true) {
        let mensagem = "Dw 2";
        console.log(mensagem);
    }
    console.log(mensagem);
}

funcao();
```
Se a variável for acessada de dentro do if, irá dizer "Dw 2", mas se for acessada de fora do if, dirá "Hello world"

## Escopo de Função
Variáveis que foram criadas dentro de uma função são acessíveis somente dentro da função

## Exemplo
```javascript
function funcao() {
    var mensagem = "DW 2";
    console.log(mensagem); 
}
console.log(mensagem);
```
isso resultará em um erro, pois a manesagem foi definida dentro da função, e não pode ser acessada fora dela, para funcionar, deve-se chamar a função ao inves disso
```javascript
function funcao() {
    var mensagem = "DW 2";
    console.log(mensagem); 
}
funcao()
```

# Tipos de dados

## Tipos Primitivos
Os tipos de dados primitivos são tipos de dados simples e imutáveis e existem vários tipo, como string, boolean, undefined, null e number.

## Number
O tipo de dados primitivos Number serve para ilustrar números, tanto inteiros quanto racionais, como por exemplo 5, -5, e 3.14.
```javascript
//Declaração
let idade = 30; 
let altura = 1.75;
console.log(idade);
console.log(altura);

// operações
let soma = 10 + 5;
let multiplicacao = 20 * 3;
let divisao = 100 / 4;

console.log(soma);
console.log(multiplicacao);
console.log(divisao);
```

## Boolean
O tipo de dados primitivos Boolean é um tipo de dado que possui 2 valores possíveis, sendo eles 0 e 1, sendo eles true e false.
```javascript
let ensolarado = true;
let chuva = false;

console.log(ensolarado);//true
console.log(chuva);//false
```

## String
O tipo de dados primitivos String serve para ilustrar cadeias de caracteres, como mensagens, como por exemplo "Hello world".
```javascript
let mensagem = "Hello world"
let mensagem2 = "Dw 2"
console.log(mensagem, mensagem2)
```

## Undefined 
O tipo de dados primitivos Undefined serve para valores indefinidos, e é geralmente atribuído automaticamente a variáveis que foram definidas mas não foram inicializadas.
```javascript
//variavel undefined
let variavelIndefinida;
console.log(variavelIndefinida);
//função não definida
function funcao() {
}

let resultado = funcao();
console.log(resultado); 
```
## Null
O tipo de dados primitivos Null é usado para os dados que foram intecionalmente deixados com valor nulo.
```javascript
//variavel null
let nulo = null;

console.log(nulo);

//alteração pra null
let numero = 10;
numero = null;
console.log(numero);
```