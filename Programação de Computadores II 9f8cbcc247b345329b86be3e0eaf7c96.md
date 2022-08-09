# Programação de Computadores II

## Linguagem de Programação

Java

![https://s2.glbimg.com/q-0B1SbZWYgxxnLwsf6dbXgivj4=/696x390/smart/filters:cover():strip_icc()/i.s3.glbimg.com/v1/AUTH_08fbf48bc0524877943fe86e43087e7a/internal_photos/bs/2021/P/f/y52r4ySZWLkJjEhKLhgw/2014-11-14-java-logo.jpg](https://s2.glbimg.com/q-0B1SbZWYgxxnLwsf6dbXgivj4=/696x390/smart/filters:cover():strip_icc()/i.s3.glbimg.com/v1/AUTH_08fbf48bc0524877943fe86e43087e7a/internal_photos/bs/2021/P/f/y52r4ySZWLkJjEhKLhgw/2014-11-14-java-logo.jpg)

## O que é Java?

O Java é uma **linguagem de programação orientada a objetos.**

Diferente da Linguagem C, toda a programação feita em Java é baseada em cima de Classes e Objetos. 

As Classes se assemelham a objetos no mundo real e podem possuir **atributos** e **métodos**. Com este recurso é possível criar vários Objetos em seu algoritmo e utilizar dos métodos e atributos fornecidos pela Classe. Pense nela como um modelo para criação dos Objetos.

## Teoria e Prática

### 1) Declaração, Tipos de Variáveis, Escrever na Tela e Ler Teclado

### Sintaxe

`Tipo_da_Variavel + Nome_da_Variavel`

### Tipos

`int` - Usado para atribuir valores inteiros;

`double` - Usado para atribuir valores decimais;

`char` - Usado para atribuir um caracter;

`String` - Usado para atribuir uma string;

`boolean` - Usado para atribuir valores booleanos (True ou False).

### String e char

<aside>
⚠️ Atenção especial para os tipos `String` e `char` . Os valores destes tipos devem ser atribuídos dentro de aspas. Um caracter em `a` (aspas únicas) e uma string em "Ola" (aspas duplas).

</aside>

### Escrever na Tela

Para conseguirmos visualizar o valor de uma variável temos que informar o programa a função necessária para isto: `System.out.println();`

Sobre esta sintaxe, ficará melhor explicado na aba de Classes.

<aside>
⚠️ Atenção na hora de colocar caracteres e Strings novamente, pois será necessário o uso de aspas únicas e aspas duplas assim como na tipagem acima.

</aside>

**Concatenação:** Quando quiser mostrar mais de uma variável no mesmo comando, ou apenas juntar vários valores, use concatenação dentro do comando `System.out.println()` que é definido pelo caracter `+` .

### Exemplo

```java
//Tipo + Nome
int num;
double num_dec;
char letra;
String nome;
boolean resposta;

num = 2;
num_dec = 5.3;
letra = 'a';
nome = "Bernardo Lucas";
resposta = True;

System.out.println("O valor da variável é: " + num);
```

### 2) Estrutura Condicional e Operadores

### Operadores Lógicos

`<` - menor que

`>` - maior que

`<=` - menor ou igual

`>=` - maior ou igual

`==` - comparação

`&&` - “and” Estabelece que duas (ou mais) condições tem que se satisfazerem simultaneamente para uma resposta booleana positiva

`||` - “or” Estabelece que apenas uma das duas (ou mais) condições tem que ser satisfeitas para uma resposta booleana positiva

`!` - “not” Estabelece que a resposta booleana encontrada será invertida

### Condicionais

A Estrutura Condicional tem o objetivo de comparar dois ou mais argumentos e decidir se o conteúdo do bloco será executado ou não por meio de uma resposta booleana.

### Tipos

`if` - “se” Compara dois ou mais argumentos e retorna uma resposta booleana

`else if` - ”se não” Usado quando mais de uma condição é necessária. 

`else` - Usado como última opção executável caso nenhuma das outras condições forem satisfeitas.

### Sintaxe

`if(){}` - Dentro dos parênteses vão os argumentos de comparação e dentro das chaves vai o código de execução caso as condições forem satisfeitas.

`else if(){}` - Caso haja mais de uma condição, talvez esta sintaxe seja mais adequada nas próximas comparações.

`else{}` - Esta sintaxe não necessita de argumentos, pois ela será executa apenas se todos os outros if não forem satisfeitos.

### Exemplo

```java
int num1 = 5;
int num2 = 5;

//estrutura if para comparar se num1 é maior que num2
if(num1 > num2) {
	System.out.println("É maior!");
} else{
	System.out.println("Não é maior!");
}

//agora vamos fazer mais de duas comparações e definir o que de fato num1 é de num2
if(num1 > num2) {
	System.out.println("É maior!");
} else if(num1 < num2) {
	System.out.println("É menor!");
} else{
	System.out.println("É menor!"); //de fato esta será a execução correta
}

```

### 3) Estrutura de Repetição

<aside>
👉🏽 Estas estruturas se fazem necessárias todas as vezes que sentir que uma linha de código está se repetindo ao longo do algoritmo.

</aside>

### Tipos e Sintaxe

`while(){}` - Este laço executará um loop conforme as condições passadas em seus parênteses;

`for( ; ; ){}` - Este laço é utilizado quando as condições de loop se resumirem a um simples intervalo. Note que este loop possui três parâmetros.

O primeiro é o valor inicial da variável iteradora (explicada logo abaixo). Ex: `i = 0`;

O segundo é o limite a qual esta variável poderá chegar, ou seja, mais precisamente a quantidade de vezes que este loop irá girar. Ex: `i < 5`;

O terceiro é onde ocorre a adição de 1 unidade à variável iteradora a cada vez que o loop gira. Ex: `i++` ou `i = i + 1`.

### Variável Iteradora

A variável iteradora, comumente chamada de `i` ou `temp` , tem como função iterar um dado intervalo. Por exemplo:

```java
//primeiro criamos a variável iteradora e definimos seu valor como 0
int i = 0;

//depois estipulamos um intervalo para ela iterar dentro do laço
while(i < 10) {

	...

	//como última linha do laço, nós iteramos a variável em 1
	i = i + 1;
}
```

Desta forma, este loop irá funcionar até que a iteração da variável `i` chegue a 10 e, para isso, a cada volta do loop a variável tem a unidade 1 acrescentada a seu valor original.

### Controladores de Laço

`continue` - todas as vezes que esta linha de código for lida, o loop passará para a próxima repetição ignorando possíveis linhas de código abaixo deste comando;

`break` - diferente do continue, quando esta linha de código for lida, o programa sairá do loop e seguirá para outras linhas de código fora do loop, independente das linhas de código restantes dentro do loop.

### Exemplo

```java
//Exemplo do laço for
int i;

for(i = 0; i < 10; i++) {
	//código
}
/*note que não é necessário adicionar 1 unidade a variável iteradora ao fim do loop
e nem dar valor 0 na criação da variável pois isto já ocorre nos argumentos do 
cabeçalho*/

//Exemplo while
int i = 0;

while(i < 10) {
	//código
	i = i + 1;
}

//Exemplo continue e break;
int i;

//Este algoritmo irá printar todos os números que a variável iteradoraa assume.
//Porém, quando ela for igual a 4, o programa irá pular para a próxima repetição
//ignorando o print abaixo.
for(i = 0; i < 10; i++) {
	if(i == 4) {
		continue;
	}
	System.out.println(i);
}

//Este algoritmo, parecido com o de cima, irá printar todos os números que variável
//iteradora assume até o 3, pois quando ela assumir o valor 4, o comando break será
//executado e o programa sairá deste loop independente do intervalo inicial estipulado.
for(i = 0; i < 10; i++) {
	if(i == 4) {
		break;
	}
	System.out.println(i);
}
```

### Laços Encaixados

Dependendo da questão pedida, será necessário utilizar um laço dentro do outro. Um exemplo é a **Manipulação de Matrizes [i][j],** em que um laço manipula as linhas **[i]** e o outro laço manipula as colunas **[j].** Neste caso, `i` e `j` são as variáveis iteradoras.

### 4) Vetores e Matrizes

### Conceito

Quando precisamos adicionar mais de um valor a uma mesma variável se faz a necessidade dos ***vetores***, ou até ***matrizes*** dependendo da aplicação.

Pode-se definir os vetores como uma lista de elementos sob uma mesma variável. Assim como as variáveis, os vetores e matrizes tem os mesmos tipos (*int*, *double*, *char*, *String*, *boolean*).

Estes elementos dizem a respeito a uma Classe importante chamada Array, porém, este assunto será abordado em outra aula, e por isso alguns termos e sintaxes desconhecidas estarão presentes, como o `new` .

### Sintaxe

`int[] vet1 = new int[10]` - A semelhança com a criação de variáveis simples é grande, porém há algumas diferenças. A primeira delas é a presença dos colchetes no tipo `int[]` . Os colchetes são a indicação de transformação de uma variável simples em vetor (ou matriz). A próxima diferença é a atribuição do `new` e logo após o tipo novamente acompanhado dos colchetes e dessa vez um valor `int[10]`. Esta atribuição significa que você está instanciando a sua variável do tipo int como um Array de tamanho 10.

Esta definição ficará mais clara no capítulo de Classes. Por agora, tudo o que precisa saber é que a instanciação contém o tamanho de seu vetor (ou matriz).

`int[][] mat1 = new int[3][5]` - Assim como o vetor, a matriz segue a mesma sintaxe e instanciação com tamanhos. Sua diferença é a presença de um segundo par de colchetes para definir as linhas.

<aside>
👉🏽 Vale lembrar que estas estruturas podem ser criadas com outros tipo além do *int. Ex: `String[] a = new String[6]`*

</aside>

### Acesso

Após criado o vetor (ou matriz), vamos acessa-lo.

Instanciado um vetor de tamanho 5 `double[] notas = new double[5]`, podemos entendê-lo como uma caixa com cinco repartições nomeadas com índices, começando pelo zero. Por exemplo:

| 0 | 1 | 2 | 3 | 4 |
| --- | --- | --- | --- | --- |
| - | - | - | - | - |

Note que os slots só vão até o 4, pois começam no 0. O tamanho do vetor é 5, mas os slots vão de 0 a 4.

<aside>
⚠️ O último slot de um vetor de tamanho *n* será *n - 1.*

</aside>

A primeira linha são os índices de cada slot da caixa, e a segunda linha são os slots associados a cada índice, ou seja, para inserir um valor no primeiro espaço do vetor, basta acessar o índice 0 e determinar o valor ali presente. Ex: `notas[0] = 2.5`

| 0 | 1 | 2 | 3 | 4 |
| --- | --- | --- | --- | --- |
| 2.5 | - | - | - | - |

```java
notas[1] = 3.2;
notas[2] = 7.8;
notas[3] = 3.3;
notas[4] = 8.0
```

| 0 | 1 | 2 | 3 | 4 |
| --- | --- | --- | --- | --- |
| 2.5 | 3.2 | 7.8 | 3.3 | 8.0 |

Analisando esta sentença de código e relembrando o capítulo de `Estrutura de Repetição` percebe-se que há uma necessidade de um loop, pois há constante repetição da mesma linha de código.

Desta forma, vamos percorrer o vetor com a variável iteradora. Ela fará papel de índice a cada repetição.

```java
for(i = 0; i < 5; i++) {
	notas[i] = 0;
}
//Desta forma estamos atribuindo 0 a todos os índices do vetor.
```

| 0 | 1 | 2 | 3 | 4 |
| --- | --- | --- | --- | --- |
| 0 | 0 | 0 | 0 | 0 |

Para as matrizes os casos são bem parecidos.

Instanciada uma matriz quadrada de tamanho 3 `String[][] nome = new String[3][3]` , vamos entender como funciona sua “caixa de slots”.

| (i, j) | 0 | 1 | 2 |
| --- | --- | --- | --- |
| 0 | - | - | - |
| 1 | - | - | - |
| 2 | - | - | - |

O acesso da matriz é por meio de coordenadas (i, j), onde i são as linhas e j as colunas, ou seja, `nome[1][2] = “Bernardo”` é o acesso da linha 1 e coluna 2.

| (i, j) | 0 | 1 | 2 |
| --- | --- | --- | --- |
| 0 | - | - | - |
| 1 | - | - | Bernardo |
| 2 | - | - | - |

Da mesma forma, precisamos de um loop para acessar toda a matriz de forma mais simples e otimizada, e, como foi falado no capítulo de `Estruturas de Repetição` , as matrizes utilizam do método de *Laços Encaixados*.

```java
int i, j;

for(i = 0; i < 3; i++) {
	for(j = 0; j < 3; j++) {
		nome[i][j] = "Sem nome";
	}
}
//Neste caso o algoritmo está atribuindo a string "Sem nome" para todos os slots
```

Enquanto o primeiro laço mantém a variável iteradora `i` em 0, o segundo laço percorre todo o intervalo de 0 a 2 com a segunda variável iteradora `j` . Quando o segundo laço terminar sua execução ele irá avançar para a próxima linha de código, que na verdade ainda é o primeiro laço. Então, a variável iteradora `i` agora valerá 1 e o programa adentrará o segundo laço novamente, o fazendo percorrer todo o intervalo pela segunda vez. Este processo irá se repetir até que o primeiro laço criado termine seu intervalo.

| (i, j) | 0 | 1 | 2 |
| --- | --- | --- | --- |
| 0 | Sem nome | Sem nome | Sem nome |
| 1 | Sem nome | Sem nome | Sem nome |
| 2 | Sem nome | Sem nome | Sem nome |

Deste modo, é possível **percorrer toda uma matriz pelas linhas e colunas.**

### Exercícios

- **Exercícios Cap. 1 e 2**
    
    **1)** Construa um algoritmo que compare dois números e imprima o maior deles.
    
    **2)** Construa um algoritmo que receba o ano e o semestre do aluno. Se o ano for 2022 e o semestre for 1, imprima: **calouro.** Caso contrário imprima: **veterano.**
    
    **3)** Dada a tabela:
    
    | 562 | Sinais e Sistemas |
    | --- | --- |
    | 034 | Fisica IV |
    | 552 | Circuitos Eletricos |
    | 429 | AEDSII |
    | 466 | Teoria dos Grafos |
    
    Construa um algoritmo que receba o código e imprima a disciplina correspondente. Faça uma condição extra caso for inserido um código que não há na tabela.
    
    **4)** Construa um algoritmo que se assemelhe a uma calculadora. O programa deve receber dois números e um caracter. Se o caracter for ‘+’, o algoritmo deve somar os dois números, se for ‘-’ deve subtrair, se for ‘*’ deve multiplicar, e se for ‘/’ deve dividir.
    
    **5)** Construa um algoritmo que dado um valor em metros, converte-lo para centímetros.
    
    **6)** Construa um algoritmo que dado um valor em Fahrenheit, realize a conversão para Celsius. Utilize esta fórmula: $C=(f-32.0) * (5.0/9.0)$.
    
    **7)** Construa um algoritmo que receba o valor de um produto. Inflacione o valor do produto em 10% caso o valor for menor ou igual a R$100, e em 20% caso for maior do que R$100.
    
- **Exercícios Cap. 3 e 4**
    
    **1)** Construa um algoritmo que, dado um vetor de tamanho *n*, encontre a média aritmética e a escreva na tela. Utilize **estruturas de repetição** para preencher e fazer os cálculos nos vetores.
    
    **2)** Construa um algoritmo que, dado um vetor de inteiros de tamanho *n*, preencha-o com valores aleatórios (o tamanho do vetor deve ser escolhido durante a execução do programa). Crie um segundo vetor (de mesmo tamanho) e armazene em cada slot o dobro dos valores do primeiro vetor. **Exemplo: vet1[0] = 3 || vet2[0] = 6**. Utilize **estruturas de repetição** para preencher e fazer os cálculos nos vetores.
    
    **3)** Construa um algoritmo que realize uma busca dentro de um vetor *n* por um número (inteiro positivo) de sua escolha e escreva na tela o número e sua posição dentro do vetor caso ele exista. Caso contrário, escreva uma mensagem informando a inexistência deste número e peça para o usuário digitar outro número. O programa só **termina quando o usuário digitar um número negativo**. Utilize **estruturas de repetição** para preencher os vetores.
    
    **4)** Construa um algoritmo que, dada uma matriz quadrada *n*, calcule a determinante e imprima na tela. Cálculo da determinante: `produto da diagonal principal - produto da diagonal secundária = determinante` . Dica: **desenhe a matriz em uma folha de papel juntamente com suas coordenadas, e avalie as coordenadas dos números da diagonal principal e diagonal secundária e encontre a lógica de cada um.**