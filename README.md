### JAVASCRIPT: ESTUDANDO LÓGICA DE PROGRAMAÇÃO 

* Estilo de declaracao de nome de variavel para JavaScript é camelCase, 1a letra minuscula 2a letra maiuscula.

* JS é linguagem não tipada, não é necessario declarar o tipo da variavel antes de declarar.

### VARIAVEIS 
* let + NomeDaVariavel [declaração de variável, alterável ao longo do codigo]

* const [declaracao de constante, inalterável ao longo do código]

### SINTAXE BÁSICA 
* console.log [print terminal]

* // [comentário]

+ [concatenação]

* " " [texto]

* ' ' [caracter]

### TIPAGEM DE VARIÁVEIS:

1. Strings [var armazena texto]
2. Numbers [var armaeza numero]
3. Booleans [var booleana - true or false]

### ESTRUTURA DE DADOS 
1. **VETORES** [item1, item2, item3]
* Pode declarar diferentes tipos de VARIÁVEIS,
os dados podem ser de tipos misturados.

* Não é necessário declarar o tipo de vetor:

**exemplo**: 
let nomeUsuarios = ["nome1", "nome2", "nome3"]

//Print valor especifico dentro do vetor:
console.log(nomeUsuarios[1]) //printa nome2

**Vetores também possuem métodos ou funções**

.pop() [remove ultimo elemento do vetor]

.shift () [remove primeiro elemento do vetor]


2. **MATRIZES**
Matrizes podem ser declaradas como conjuntos de arrays que vão formando as linhas e colunas e 
podem armazenar diferentes tipos de dados no mesmo array. É preferível usar matriz quando os dados são de diferentes tipos.

**Exemplo:** Matriz 2 x 3

let todosUsuarios = [

    ["maria", "20 anos", "SC"],
    ["Joao", "23 anos", "SP"],
]

console.log(todosUsuarios[0]) //imprime a linha
    
    ["maria", "20 anos", "SC"]

console.log(todosUsuarios[0][0]) //imprime a linha 0 e conteudo que está no indice 0 do array:
    
    Maria
 

 **Exemplo:** Matriz 3 x 3 

 let timePokemon = [
     
     ["Pikachu", 20, "SC"],
     ["Char", 23, "SP"],
     ["Bulba", 25, "RJ"]
]

console.log(timePokemon[0][1])

**Resultado:**
20

console.log(timePokemon[0])

**Resultado:**

(3) ["Pikachu", 20, "SC"]

console.log(timePokemon[2])

**Resultado:**

(3) ["Bulba", 25, "RJ"]

console.log(timePokemon[2][1])

**Resultado:**
25


### MÉTODOS .  [COR ROXA]
serve para array e matrizes, ações que podem ser feitas.

nome array ou matriz . [aparecem funções//metodos que podem ser feitos com a variavel. Executam ações]

**exemplo:**

let nomeUsuarios = ["nome1", "nome2", "nome3"]

nomeUsuarios.pop [remove ultimo elemento do array = nome3]


### PROPRIEDADES .  [COR AZUL]
serve para array e matrizes, caracteristicas da estrutura sendo utilizada.

nomeDaEstrutura.length [quantas posições array possui]


### Operadores Aritméticos:

| Operador | Descrição | Exemplo |
| --- | --- | --- |
| + | Adição | let result = 5 + 3; |
| - | Subtração | let result = 8 - 2; |
| * | Multiplicação | let result = 4 * 6; |
| / | Divisão | let result = 10 / 2; |
| % | Módulo (resto da divisão) | let result = 10 % 3; |

### Operadores Relacionais:

| Operador | Descrição | Exemplo |
| --- | --- | --- |
| == | Igual a | let isEqual = (x == y); |
| != | Diferente de | let isNotEqual = (x != y); |
| > | Maior que | let isGreater = (x > y); |
| < | Menor que | let isLess = (x < y); |
| >= | Maior ou igual a | let isGreaterOrEqual = (x >= y); |
| <= | Menor ou igual a | let isLessOrEqual = (x <= y); |

### Operadores Lógicos:

| Operador | Descrição | Exemplo |
| --- | --- | --- |
| && | AND lógico | if (condition1 && condition2) |
| || | OR lógico | if (condition1 || condition2) |
| ! | NOT lógico | if (!condition) |

### Operadores de Atribuição:

| Operador | Descrição | Exemplo |
| --- | --- | --- |
| = | Atribuição | let x = 5; |
| += | Adição e atribuição | let num = 10; num += 2; |
| -= | Subtração e atribuição | let num = 10; num -= 3; |
| *= | Multiplicação e atribuição | let num = 5; num *= 4; |
| /= | Divisão e atribuição | let num = 10; num /= 2; |
| %= | Módulo e atribuição | let num = 10; num %= 3; |

### Operadores de Incremento e Decremento:

| Operador | Descrição | Exemplo |
| --- | --- | --- |
| ++ | Incremento | let counter = 0; counter++; |
| -- | Decremento | let counter = 5; counter--; |


# JavaScript [PART 2]

# Estruturas condicionais IF ELSE | ELSE IF (ENCADEADO)
Var booleana ou expressao que retorna bool 
---------------------------------------------
if (condição){
    faz tal coisa 
}

---------------------------------------------
If (condição){

    faz tal coisa
}
else {
    faz outra coisa
}
---------------------------------------------
>>>>>>>>>>>>>>>>>>>> if encadeado
If (condição){

    faz tal coisa
}
else if {
    faz outra coisa
}
else if {
    faz outra coisa
}
else{

}

_______________________________________________________________
# SwitchCase [Estrutura de Decisão]
Muitas casos para testar é melhor usar o SWCASE, 
também pode ser feito com o IF, Else If, Else. 

palavras chave > switch case break, default.
Pode-se ter mais de um case no mesmo bloco, basta colocar
um case em cima do outro. O break auxilia em parar a execução 
ao encontrar variavel igual ao caso testado. 
---------------------------------------------
switch (expression) {
  case caseExpression1:
    statements
  case caseExpression2:
    statements
    break;
  case caseExpressionN:
    statements
    break;
  default:
    statements
}

_______________________________________________________________
Laços de Repetição : mais utilizado

1. for : repetir ação várias vezes. Verificação contínua.
variavel i usada como iterador
    for (condicao inicial, cond parada, incremento){
            ação a ser feita repetidamente;
    }

    for (i=0;i<valor parada; i++){
        console.log(i);                 //conta até valor de parada 
    }

2. While : alternativa do for. Até uma determinada condição ser satisfeita
>>> condição é mais direta, exemplo de condição count < 3  ou i < 3 [interador]
contador ou interador deve ser incrementado dentro do while. 

while (condição){
    console.log("mensagem");
    condição++ //deve incrementar o contador
}

3. Do While : faz algo até certa condição de parada. 

do {
    ação ();
    itera contador ou i; 
}
while (contador ou iterador) //regra para parar
