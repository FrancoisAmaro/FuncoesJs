# FuncoesJs
1ª atividade da disciplina Linguagens de Script - IFPB - TSI - 2025_2

<ins>Tutorial para definir e criar funções em JavaScripit utilizando os formatos: declaration, expression e arrow.</ins>

E aí companheiro dev, tudo bom? Aqui você saberá um pouco sobre o conceito e exemplos de funções em Javascript. Você deve ser ~~veterano~~ iniciante assim como eu, então vamos iniciar essa jornada juntos. Funções permitem organizar, reutilizar e tornar tudo mais eficiente. Assim, iremos abordar 3 tipos: *declaration, expression e arrow.*

## Declaration

A maneira mais simples de definir funções em JavaScript é através da function declaration, toda função de declaração começa com a palavra reservada e obrigatória function, seguida pelo nome da função (também obrigatório) e uma lista de parâmetros (opcionais) separados por vírgula e encapsulados em parenteses (obrigatórios), o último passo é definir as chaves (obrigatórias) que será o corpo da função.
Exemplo:
  ![Declaration1](https://private-user-images.githubusercontent.com/187148916/498878651-583354f9-13f1-4fe8-bbbe-e105bb2c8980.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTk5MzI0OTgsIm5iZiI6MTc1OTkzMjE5OCwicGF0aCI6Ii8xODcxNDg5MTYvNDk4ODc4NjUxLTU4MzM1NGY5LTEzZjEtNGZlOC1iYmJlLWUxMDViYjJjODk4MC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMDA4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTAwOFQxNDAzMThaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00ZTg5NTkyNTg3ZTFjYjEzZjRlYTZkZTMyNDlmODRhNThkYTkyNzhiNzIyODZkZWFhYjViNmE2MDE3NjEwNzhiJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.HzBC_5ZjWKi9hexZB23FdTasircFWSfT-htBSZ6MY1Q)

Essa estrutura é a mais simples, porém, obrigatória para as functions declaration.Como mencionado anteriormente, também podemos definir parâmetros opcionais separados por vírgula

![Declaration02](https://private-user-images.githubusercontent.com/187148916/498879004-013d6145-7f95-47c4-8ed3-e46b04ed5efa.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTk5MzI0MDIsIm5iZiI6MTc1OTkzMjEwMiwicGF0aCI6Ii8xODcxNDg5MTYvNDk4ODc5MDA0LTAxM2Q2MTQ1LTdmOTUtNDdjNC04ZWQzLWU0NmIwNGVkNWVmYS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMDA4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTAwOFQxNDAxNDJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT04MDc2MmY4NDEwNDcyMzQ3OTU2YTQzYmExYjM3ZTEyMTM0N2NmOGEwODNmNzVkYTAyZTliOTQyNGZhZGFiMDc2JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.RwXyFpNHp2YlrRt42VYlCFE3AYSeEIWfHkpHhXRtQmg)

## Vantagens
-Hosting.  
-Legibilidade do código.  
-Facilidade de depuração.  

## **Desvantagens**
-Hoisting, apesar de ajudar, pode causar problema em códigos maiores.  
-Sem função anônima.  

## **Exemplo 1**  
```javascript
Function square(numero){  
	Return numero*numero;
}  
```

## **Exemplo 2**  
```javascript
//Declaração de funções em JavaScript são hoisted à definição de função. Pode usar uma função antes de tê-la declarada
Hoisted();  

Function hoisted(){  
	Console.log(“FOO”);  
}  
```
## **Exemplo 3**  
```javascript
Function nome (Francois){  
	Console.log(‘nome’, Francois)  
}  
nome(‘Francois’)  
```
## Expression  
Uma expressão  de função (function expression) se difere de uma declaração de função tradicional na forma a qual 
declaramos um nome a uma variável podendo ser uma função anônima. A função de expressão pode ser lidada como uma qualquer expressão em JavaScript, por exemplo:  
```javascript
const nome = 'Francois'  
```
Nesse exemplo, estamos criando uma expressão onde definimos uma variável chamada nome e atribuímos uma String para ela.
Com as funções de expressão, podemos fazer algo muito semelhante:  
```javascript
const ola = function() {  
    console.log('Olá')  
}  
ola()  
```
![Expression](https://private-user-images.githubusercontent.com/187148916/498879331-6e5e879d-32dd-46ab-973c-e2bce0fded98.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTk5MzI4NzksIm5iZiI6MTc1OTkzMjU3OSwicGF0aCI6Ii8xODcxNDg5MTYvNDk4ODc5MzMxLTZlNWU4NzlkLTMyZGQtNDZhYi05NzNjLWUyYmNlMGZkZWQ5OC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMDA4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTAwOFQxNDA5MzlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT05YjljNmYwOGY2YjdiNWYwYTIzOWUzMGNiZTZiMGIzY2NkNDM2YTlhODQzZjg3MzE4Y2RkN2YxY2VkY2U2N2U4JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.SYpPEtyT0fQ4-VeA54IwRJqGbFjKM35zuuZATbgrelY)


Repare que é bem parecido com as funções de declaração, uma das sútis diferenças é que ela está sendo atribuída para uma variável, 
onde não definimos o nome da função e sim o nome da variável que irá referenciar a mesma.
 

## **Vantagem**  
-Pode criar funções anônimas.   
-Legibilidade do código.  



## **Desvantagem**  
-Não faz hosting.  
-Depuração menos clara (caso seja uma função anônima).  

## **Exemplo 1**  
```javascript
var x= function (y){  
	return y*y;  
};  
```
## **Exemplo 2** - Função anônima
```javascript 
Let saudação= function (nome){  
	Return ‘olá,$ {nome}!’;  
};
Console.log(saudação ‘Francois’);  
```
## **Exemplo 3**  
```javascript
const gerarnome= function(nome){  
	return’ OI, meu nome é ${nome}’;  
};  
const francois=gerarnome(“Francois");  
console.log(francois);  
```
## Arrow  
Uma expressão arrow function(funções de seta) tem uma sintaxe pequena, um dos motivos da 
criação desta função é facilitar a criação e utilização de funções em JavaScript, ou seja, elas permitem a criação de funções de maneira resumida. 
Em vez de function palavra-chave, ela usa uma seta (composta por dois sinais: = e >).


![Seta01](https://github.com/user-attachments/assets/585c33f0-865b-46b4-b531-812e01d74e13)

## Vantagens  
-Sintaxe pequena.  
-São anônimas.  


## Desvantagens.  
-Método de objetos.  
-Não faz hosting.  

## Exemplo 1 
```javascript
const n1 = Number(prompt("Digite o 1º número:"));
const n2 = Number(prompt("Digite o 2º número:"));

const soma = (c, d) => {
    return c + d;
};

console.log("Resultado da soma:", soma(n1, n2));
```
## exemplo 2
```javascript
const ola = () => {
    console.log("Olá, mundo!");
};

ola(); 
// Chamando a função para que ela seja executada
```
## exemplo 3
```javascript
const mult = (x, y) => {
    const valor = x * y;
    return valor;
};

console.log("Resultado da multiplicação:", mult(2, 3));
```






