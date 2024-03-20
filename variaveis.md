# Declaração de variáveis 
### Para se declarar uma variável, podem se usar 3 comandos diferentes, let, var, e const, cada um com suas funções
## Let
O comando let é utilizado para criar uma variável e limitar o seu escopo em um bloco ou expressão onde ela é usada
### Exemplo Let:

    let message = "Hello world";

    message = " Dw2";

    alert(message);


## Var
O comando var é utlizado para criar uma variável com escopo global, sendo visível em todo o código, Var é menos utilizado devido a seus problemas de escopo, que são mais fáceis de se controlar com os outros comandos
### Exemplo var
```
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
 O comando const é utilizado para se criar variáveis que não podem ter seus valores alterados ou reatribuídos, sendo imutáveis, qualquer tentativa de alteração de valor resultará em um erro.
 ## Exemplo erro
 ```
const PI = 3.14159;
PI = 3;
```
## EXEMPLOS
```
//declarando
const nome = "Alice";
const idade = 30;

// Declarando uma variável com um objeto
const pessoa = {
    nome: "João",
    idade: 25
};

// Modificar um atributo da variável é permitido
pessoa.idade = 26;

//Tentativa de reatribuir (vai dar erro)
pessoa = { nome: "Maria", idade: 35 };

// Exibir os valores

console.log(PI);
console.log(nome);
console.log(idade);
console.log(pessoa);
```
