**Ponteiros na linguagem C**

A utilização de ponteiros em linguagem C é uma das características que tornam a linguagem tão flexível e poderosa. Ponteiros ou apontadores, são variáveis que armazenam o endereço de memória de outras variáveis.Dizemos que um ponteiro “aponta” para uma varíável quando contém o endereço da mesma. Os ponteiros podem apontar para qualquer tipo de variável. Portanto temos ponteiros para int, float, double, etc.

**Por que usar ponteiros?**

Ponteiros são muito úteis quando uma variável tem que ser acessada em diferentes partes de um programa.Neste caso, o código pode ter vários ponteiros espalhados por diversas partes do programa, “apontando” para a variável que contém o dado desejado.

Caso este dado seja alterado, não há problema algum, pois todas as partes do programa tem um ponteiro que aponta para o endereço onde reside o dado atualizado.

Existem várias situações onde ponteiros são úteis, por exemplo:

- Alocação dinâmica de memória
- Manipulação de arrays.
- Para retornar mais de um valor em uma função.
- Referência para listas, pilhas, árvores e grafos.

**Sintaxe de declaração de ponteiro**

**tipo \*nome_ponteiro;**

Onde temos:

**tipo** : é o tipo de dado da variável cujo endereço o ponteiro armazena.

***nome_ponteiro** : O nome da variável ponteiro.

O asterisco * neste tipo de declaração determina que a variável será um ponteiro.

Exemplo de declaração de ponteiro:

**int \*ptr;**

**Exemplo: Programa utilizando ponteiro**

\1.    **#include <stdio.h>**

\2.    **#include <conio.h>**

\3.     

\4.    **int** **main**(**void**)

\5.    {

\6.    //valor é a variável que

\7.    //será apontada pelo ponteiro

\8.    **int** valor = 27;

\9.     

\10. //declaração de variável ponteiro

\11. **int** *ptr;

\12.  

\13. //atribuindo o endereço da variável valor ao ponteiro

\14. ptr = &valor;

\15.  

\16. **printf**("Utilizando ponteiros\n\n");

\17. **printf** ("Conteudo da variavel valor: %d\n", valor);

\18. **printf** ("Endereço da variavel valor: %x \n", &valor);

\19. **printf** ("Conteudo da variavel ponteiro ptr: %x", ptr);

\20.  

\21. **getch**();

\22. **return**(0);

\23. }

A disponibilidade do uso de ponteiros em C++ agrega um poder a mais ao conjunto da linguagem, porém implica a necessidade de cautela na elaboração de programas que usam deste recurso. Certamente, nem todos os programadores precisam ser considerados inaptos, a priori, através da supressão ou inserção de complicadores de recursos criados explicitamente para forçá-los a não usar dos recursos. Por isso, a linguagem C++ disponibiliza o recurso para quem deseja utilizá-lo e também apresenta diversos outros recursos que são alternativas ao uso de ponteiros quando eles não são imprescindíveis.


 Exemplo:

```c
           int *px;
```

​        **Tipos por referência (JAVA)**

Os programas utilizam as variáveis de tipos por referência para armazenar as localizações de objetos na memória do computador. Esses objetos que são referenciados podem conter várias variáveis de instância e métodos dentro do objeto apontado.

Para trazer em um objeto os seus métodos de instância, é preciso ter referência a algum objeto. As variáveis de referência são inicializadas com o valor “**null**” (nulo).

Por exemplo, ClasseConta acao = new ClasseConta(), cria um objeto de classe ClasseConta e a variável acao contém uma referência a esse objeto ClasseConta, onde poderá invocar todos os seus métodos e atributos da classe. A palavra chave new solicita a memória do sistema para armazenar um objeto e inicializa o objeto.

**Listagem 4:** Exemplo acessando um método do objeto

A saída desse código acima irá ser reproduzida através da ação acessa.imprime(), porque está sendo acessado o método do objeto que foi inicializado com a variável definida como “acessa”.

**RETORNO EM JAVA**

**O Comando return**

O comando " return" serve para sair do método em que está executando. Exemplos de uso:

```java
 public static void main(String[] args){ 
     System.out.println("Boo!");
     if (args.length > 0)
         return;
     System.out.println("Baa!");
 }
```

**Valor do Retorno**

Um método pode retornar o valor de uma variável. O tipo do valor de retorno é definido antes do nome do método. O método deve retornar um dado desse tipo através do comando **return**.

A palavra-chave **void** indica a ausência de um tipo de dado. Serve para indicar um método retorna nenhum dado. Por exemplo:

```java
public static void main(String[] args) {
  //
}
```

**Um exemplo prático**

No nosso exemplo vamos fazer métodos que realizem operações matemáticas. Suponha que vamos fazer uma classe OperacoesMatematicas:

```java
/*OperacoesMatematicas.java*/
 
public class OperacoesMatematicas{
 
   public int somar( int num1, int num2 ){
       return num1 + num2;
   }
 
   public int subtrair( int num1, int num2 ){
       return num1 - num2;
   }
 
   public int multiplicar( int num1, int num2 ){
       return num1 * num2;
   }
 
   public int dividir( int num1, int num2 ){
       return num1 / num2;
   }
 
} 
```

**RECURSIVIDADE EM JAVA**

A **recursividade** trabalha de forma similar a um laço de repetição, na verdade tudo que fazemos em laço, pode ser feito em **recursividade**. A recursividade é nada mais nada menos do que uma função dentro da outra e ela deve ser pensada como uma pilha (estrutura de dados onde o ultimo a entrar, deve ser o primeiro a sair). A estrutura dela consiste em descer até a base fazendo os cálculos ou rotinas de cada instrução, e então da base até o topo da pilha são empilhados os resultados de cada instrução e no final o topo contém o resultado que é retornado. Na figura a seguir, temos um exemplo que é frequentemente usado para explicar a recursividade, podemos encontrar em diversos livros didáticos, porque é um dos mais fáceis para se entender, estou falando do fatorial.

Ex. desenvolver um método recursivo para descobrir o fatorial de um número “N”. Suponhamos que o N seja igual a **4**.

**Obs:** O “fatorial(4)” só pode ser descoberto depois que o “fatorial(3)” for descoberto, que por sua vez só poderá ser descoberto depois do fatorial(2) e assim por diante. Por isso vai do topo até a base, e depois vai empilhando os resultados da base até o topo.

Agora uma ilustração com os valores para fixar o conceito:

![1560735928126](C:\Users\Daiane F\AppData\Roaming\Typora\typora-user-images\1560735928126.png)

![http://www.linhadecodigo.com.br/artigos/img_artigos/Ricardo_Alves/Java_Recursividade/image002.jpg](file:///C:\Users\DAIANE~1\AppData\Local\Temp\msohtmlclip1\01\clip_image002.png)

​          O conceito de recursividade como podemos ver anteriormente não é tão difícil, é claro que na hora da programação é sempre recomendável atenção, organização e fazer o tão “chato”, mas eficiente teste de mesa, ou seja, fazer o máximo para dar certo, pois a hora de errar é quando estiver treinando, fazendo exercícios e não deixar para errar quando estiver em um mercado de trabalho, onde um projeto pode ter mais de 10000 linhas.

​          Agora vamos deixar de “Blábláblá”, e vamos ao que interessa, a seguir implementaremos o exemplo do fatorial no JAVA.

Crie uma classe como a seguir:

![1560735990240](C:\Users\Daiane F\AppData\Roaming\Typora\typora-user-images\1560735990240.png)

![http://www.linhadecodigo.com.br/artigos/img_artigos/Ricardo_Alves/Java_Recursividade/image003.jpg](file:///C:\Users\DAIANE~1\AppData\Local\Temp\msohtmlclip1\01\clip_image003.png)

​          Essa é a função recursiva do fatorial em JAVA

**BIBLIOTECA**

O que é?


 Quando vc escreve um programa usando uma linguagem de programação existe a possibilidade de você usar um conjunto de funções pré-escritas por outros programadores que já resolvem determinados problemas para você sem que vc precise “reinventar a roda”. a esse conjunto de funções damos o nome de BIBLIOTECA, do inglês, library. Muitos traduzem como livraria, isso dificulta a compreensão pois livraria é uma LOJA DE LIVROS enquanto biblioteca é um conjunto de livros que vc pode usar sem precisar PAGAR.

**BIBLIOTECA jQuery**

jQuery é uma biblioteca de funções em [**JavaScript**](https://www.devmedia.com.br/guia/javascript/34372) que interage com o [**HTML**](https://www.devmedia.com.br/guia/html/38051), desenvolvida para simplificar os scripts interpretados no navegador do usuário (client-side). Criada em dezembro de 2006 no BarCamp de Nova York por [**John Resig**](https://johnresig.com/about/). Usada por cerca de 77% dos 10 mil sites mais visitados do mundo, jQuery é a mais popular das bibliotecas JavaScript.

**jQuery é uma biblioteca de código aberto (open source)** e possui licença dual, fazendo uso da [**Licença MIT**](https://pt.wikipedia.org/wiki/Licença_MIT) ou da [**GNU General Public License**](https://pt.wikipedia.org/wiki/GNU_General_Public_License) versão 2. A sintaxe do jQuery foi desenvolvida para simplificar a navegação em documentos HTML, a seleção de elementos DOM, criar animações, manipular eventos, desenvolver aplicações [**AJAX**](http://www.devmedia.com.br/introducao-ao-ajax-revista-easy-java-magazine-19/24797) e criação de plugins sobre ela. Permitindo aos desenvolvedores criarem camadas de abstração para interações de baixo nível de modo simplificado em aplicações web de grande complexidade.

Para demonstração, mostraremos um exemplo simples utilizando JQuery.



<html>

<head>

<title>Biblioteca JQuery</title>

<script type="text/javascript"
language="javascript" src="jquery-1.2.6.js"></script>

<script type="text/javascript">
***BIBLIOTECA JAR**

JAR (Java ARchive) é um arquivo compactado no formato ZIP que contém um conjunto de **classes**(arquivos “.class”) e **arquivos de configuração**. O formato JAR é utilizado para permitir a distribuição de bibliotecas ou, até mesmo, sistemas inteiros em Java (uma vez que é possível montar arquivos JAR formados por centenas de classes).

As principais bibliotecas Java desenvolvidas por terceiros – ou seja, bibliotecas que não fazem parte da JDK - são estruturadas e distribuídas em arquivos JAR. Apenas para citar alguns exemplos de bibliotecas populares, podemos relacionar: **Joda** (biblioteca para facilitar a manipulação de tipos data e hora), **XStream** (biblioteca para serializar objetos para XML), **Weka** (biblioteca de algoritmos para mineração de dados), Gson (biblioteca para serializar

### Utilizando Diversos arquivos JAR

O exemplo apresentado na seção anterior envolveu o uso de apenas um arquivo JAR. No entanto, é possível utilizar diversos arquivos, bastando separá-los por “ ; ”. Supondo que todos os JAR estejam em um mesmo diretório, a sintaxe seria similar à mostrada na Listagem 5. No exemplo, temos três arquivos JAR: “lib1.jar”, ‘lib2.jar” e “lib3.jar” e o programa “MinhaClasse.class” todos localizados na mesma pasta.

 Executando o programa

`C:\TESTE>java
-cp .;lib1.jar;lib2.jar;lib3.jar MinhaClasse`

**Referencias**

<https://www.portaleducacao.com.br/conteudo/artigos/informatica/a-biblioteca-jquery/6669>

[https://www.google.com/search?ei=MsAGXaayDabA5OUPx86lgAY&q=A+recursividade+trabalha+de+forma+similar+a+um+la%C3%A7o+de+repeti%C3%A7%C3%A3o%2C+na+verdade+tudo+que+fazemos+em+la%C3%A7o&oq=A+recursividade+trabalha+de+forma+similar+a+um+la%C3%A7o+de+repeti%C3%A7%C3%A3o%2C+na+verdade+tudo+que+fazemos+em+la%C3%A7o&gs_l=psy-ab.3..35i39l6.87355.94503..95334...1.0..0.539.2055.5-4......1....1j2..gws-wiz.....6..0i71.c7Ddnzt1Kgo](https://www.google.com/search?ei=MsAGXaayDabA5OUPx86lgAY&q=A+recursividade+trabalha+de+forma+similar+a+um+laço+de+repetição%2C+na+verdade+tudo+que+fazemos+em+laço&oq=A+recursividade+trabalha+de+forma+similar+a+um+laço+de+repetição%2C+na+verdade+tudo+que+fazemos+em+laço&gs_l=psy-ab.3..35i39l6.87355.94503..95334...1.0..0.539.2055.5-4......1....1j2..gws-wiz.....6..0i71.c7Ddnzt1Kgo)

[https://pt.wikibooks.org/wiki/Java/M%C3%A9todos](https://pt.wikibooks.org/wiki/Java/Métodos)

<https://docs.oracle.com/javase/tutorial/java/javaOO/arguments.html>