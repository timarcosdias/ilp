# Apostila de Introdução à Lógica de Programação

A **Lógica de Programação** é a técnica de encadear pensamentos para atingir determinado objetivo por meio de um computador ou outro sistema programável.

Antes de começarmos a programar, é necessário compreender novos conceitos e até rever alguns dos já vistos nas aulas de Matemática.

> Você pode acessar a versão mais atualizada deste material entrando em [github.com/timarcosdias/ilp](https://github.com/timarcosdias/ilp).

> Se encontrar erros ou tiver sugestões, por favor, envie-os para [ti.marcosdias@gmail.com](mailto:ti.marcosdias@gmail.com?Subject=Apostila de Lógica de Programação).

> Os exemplos contidos neste material adotam a sintaxe de uma variante da linguagem Portugol desenvolvida para a ferramenta [Portugol Studio](http://lite.acad.univali.br/portugol/), mantida pela UNIVALI - Universidade do Vale do Itajaí.

## 1. Algoritmo

Podemos definir algoritmo como uma sequência finita e ordenada de passos para a resolução de um problema específico.

Para exemplificar, vamos começar com um algoritmo descritivo para um problema clássico do cotidiano: como fritar ovos?

```
/*
Algoritmo para fritar ovos

1.    pegar frigideira, ovo, óleo e sal
2.    colocar óleo na frigideira
3.    acender o fogo
4.    levar a frigideira ao fogo
5.    esperar o óleo esquentar
6.    colocar o ovo
7.    colocar sal no ovo
8.    retirar quando pronto
*/
```

Percebe que o algoritmo acima é basicamente uma receita? Algoritmos são exatamente como receitas.

Uma boa recomendação para a construção de algoritmos descritivos é sempre utilizar apenas um verbo por linha, já que cada verbo geralmente indicará uma ação diferente a ser tomada.

> O nosso principal objetivo ao estudar Lógica de Programação é compreender como criar programas de computador. Um Programa de Computador nada mais é que um algoritmo escrito com o uso de uma linguagem de computador, ou linguagem de programação, como C, Pascal, Java, JavaScript, PHP etc. Há uma infinidade de linguanges de programação disponíveis mundo afora. Futuramente veremos como elas funcionam.

## 2\. Variável

Na Matemática, variável é o nome que se dá ao termo que substitui um outro desconhecido, como numa equação: `y = 2x + 1`. Em Lógica de Programação, o valor de uma variável pode ser conhecido ou não.

De forma genérica, uma variável é uma referência a um local na memória do computador, onde um valor pode estar armazenado, por exemplo: em um programa de computador, podemos ter uma variável chamada `idade`, que armazena o valor `18`.

### 2.1\. Nomenclatura de variáveis

Há algumas regras a serem seguidas ao nomear variáveis. Algumas linguanges de programação poderão apresentar padrões diferentes, mas há algumas convenções que devem ser sempre seguidas para manter o código legível e livre de erros:

- O nome de uma variável não deve conter espaços ou acentos
- O nome de uma variável não deve conter operadores
- O nome de uma variável não deve ser só um número
- Algumas linguagens de programação diferenciam letras maiúsculas de letras minúsculas, logo: `Nome` pode ser diferente de `nome`
- Variáveis cujo nome seja um substantivo composto, como "data de nascimento", **podem** ser nomeadas com o padrão camelCase: `dataDeNascimento`. Este padrão define que todas as palavras após a primeira devem começar com letra maiúscula. Outra alternativa é utilizar um traço inferior (`_`), ou underline, entre cada palavra: `data_de_nascimento`.

### 2.2\. Atribuição de valores

Atribuir um valor a uma variável é dar um valor a uma variável. É o mesmo que guardar um valor em um espaço da memória.

```
a = 4
```

Pode ser lido como: variável `a` recebe `4`.

```
nome = “José”
```

Pode ser lido como: variável `nome` recebe `José`.

Observe que o símbolo de igualdade, `=`, aqui é utilizado como operador de atribuição. Para igualdade, utilize `==`.

### 2.3\. Tipos de variáveis

O tipo de uma variável define o tipo de valor que ela poderá armazenar. Por exemplo, se precisamos armazenar um número inteiro, podemos criar uma variável do tipo **inteiro**; para armazenar nomes, utilizamos **cadeias de caracteres**.

- **Inteiro ou (int):** número inteiro. Ex.: 10 ou 50.
- **Real (float):** número real. Ex.: 10.5 ou 0.8.
- **Caracter ou Cadeia (string ou char):** número, letras, palavras e/ou outros símbolos. Ex.: "A" ou "abc123" ou "* é um asterisco.". Tenha sempre em mente que valores do tipo caractere ou cadeia de caracteres são representados entre aspas.
- **Lógico (bool):** verdadeiro ou falso, sim ou não, 1 ou 0, true ou false.

### 2.4\. Exercícios com tipos de variáveis

**1\. Informe o tipo de variável adequado para cada item abaixo:**

- a) Idade de uma pessoa
- b) Valor de uma conta de luz
- c) Nome de um cliente
- d) Estado de uma lâmpada (acesa/apagada)
- e) Senha de acesso ao Facebook
- f) Quantidade de litros de combustível abastecidos em um posto
- g) Situação de uma determinada fatura (paga/não paga)
- h) Média final de um aluno

## 3\. Operadores

Um operador é um símbolo que, como seu próprio nome diz, é utilizado para representar operações lógico-matemáticas. Os operadores que iremos utilizar são os operadores aritméticos, os operadores relacionais e os operadores lógicos. Observe que alguns deles, já utilizados na Matemática, terão seu símbolo substituído por outro na Programação.

### 3.1\. Operadores Aritméticos

- **Soma (+):** `1 + 3`
- **Subtração (-):** `5 – 4`
- **Multiplicação (*):** `8 * 8`
- **Divisão (/):** `40 / 5`
- **Resto/Módulo (%):** `20 % 3`
- **Potenciação (^):** `2 ^ 2`

### 3.2\. Operadores Relacionais

- **Igual (==):** `5 == 5`
- **Diferente (!=):** `8 != 80`
- **Maior que (>):** `12 > 11`
- **Menor que (<):** `11 < 12`
- **Maior ou igual (>=):** `18 >= 17`
- **Menor ou igual (<=):** `16 <= 16`

### 3.3\. Operadores Lógicos

- **E/Conjunção (e; &&; and):** `5 == 5 e 9 > 7`
- **OU/Disjunção (ou; ||; or):** `5 > 3 ou 7 >= 1`
- **NÃO/Negação (nao; !; not):** `nao(3 > 2) == falso`

## 4\. Tabela verdade

Uma tabela verdade é uma tabela utilizada em Lógica para verificar se uma expressão é verdadeira ou falsa.

### 4.1\. Operadores "e" e "ou"

No exemplo a seguir, temos a tabela verdade dos operadores lógicos `e` e `ou`. Observe que as variáveis `X` e `Y` representam expressões que podem ser verdadeiras ou falsas de forma independente.

![alt text](imagens/tabela-verdade1.png "Tabela Verdade 1")

Para compreender como se dá a construção dessa tabela verdade, podemos nos fazer estas duas perguntas:

- `X` e `Y` são verdadeiros?
- `X` ou `Y` são verdadeiros?

Ao questionar se `X` e `Y` são verdadeiros, questionamos se ambos são verdadeiros. Ou seja: a expressão `X e Y` só é verdadeira quando `X == verdadeiro` e `Y == verdadeiro`.

O operador `ou` já funciona de maneira diferente. Ao questionarmos se `X` ou `Y` são verdadeiros, questionamos se pelo menos um deles é verdadeiro. Ou seja: a expressão `X ou Y` é verdadeira quando `X == verdadeiro` e `Y == falso`, ou `X == falso` e `Y == verdadeiro`, ou `X == verdadeiro` e `Y == verdadeiro`.

### 4.2\. Operador "não"

O operador `não` é utilizado para negar uma determinada expressão. Ex.: se `X == verdadeiro`, então `não X == falso`; se `X == falso`, então `não X == verdadeiro`.

![alt text](imagens/tabela-verdade2.png "Tabela Verdade 2")

### 4.3\. Exercícios com tabela verdade

**1\. Complete a seguinte tabela verdade:**

![alt text](imagens/tabela-verdade-exercicios.png "Tabela Verdade - Exercícios")

## 5\. Precedência de operadores

A precedência, ou ordem, de operadores é a convenção que indica a ordem em que as operações devem ser realizadas em uma expressão. A lista abaixo descreve a ordem em que os operadores devem ser considerados:

1. Parênteses e funções
2. Potência e resto
3. Multiplicação e divisão
4. Adição e subtração
5. Operadores relacionais
6. Operadores lógicos

No exemplo abaixo, a multiplicação deve ser resolvida antes da soma.

```
3 + 4 * 9
3 + 36
39
```

Neste exemplo, a parte da expressão entre parênteses é resolvida antes da multiplicação.

```
(3 + 4) * 9
7 * 9
63
```

Quando operadores de mesma prioridade se chocam, a operação mais à esquerda prevalece sobre as demais. Ex.:

```
3 * 4 / 3
12 / 3
4
```

Neste exemplo, o operador de soma tem prioridade sobre os operadores relacionais, e os operadores relacionais têm prioridade sobre o operador lógico.

```
10 < 9 e 6 + 3 > 10
10 < 9 e 9 > 10
F e F
F
```

Para facilitar, isole as expressões que estão antes e após o operador lógico, resolva-as e só então compare seus resultados através do operador lógico.

### 5.1\. Exercícios com expressões

**1\. Indique o resultado das expressões seguindo as regras de precedência dos operadores.**

- a) `2 + 3 - 5 * 8 / 4`
- b) `7 * 4 / 2 + 9 - 6`
- c) `(4 + 2) * 3 / 4`
- d) `7 > 2 e 3 -5 < 8`
- e) `8 > 12 e 5 < 3 + 4`

## 6\. Primeiros passos em programação

Você deve ter notado no início deste material que mencionamos que a sintaxe utilizada em nossos exemplos seria a mesma de uma variante da linguagem Portugol.

Em Lógica de Programação, a **sintaxe** está ligada à **estrutura** da linguagem de programação. Ela é o conjunto de regras que definem a forma correta de composição das estruturas básicas de uma linguagem. É o que deve responder à pergunta: como construir tal estrutura corretamente?

Outro conceito que precisamos compreender é o de **semântica**. Em Lógica de Programação, a semântica está ligada ao **significado** de um determinado código. A semântica deve responder à pergunta: tal código faz realmente o que se espera que ele faça?

A seguir, são abordados alguns comandos básicos para que possamos finalmente começar a programar.

### 6.1\. Declaração de variáveis

Antes que uma variável possa ser utilizada para armazenamento de um valor qualquer, ela deve ser declarada, ou seja: precisamos reservar aquele pequeno espaço na memória do computador e nomeá-lo para uso futuro:

```
inteiro idade
```

No exemplo acima, declaramos a variável `idade` como do tipo `inteiro`.

Até que a variável `idade` seja inicializada, ou seja, até que ela receba algum valor, seu conteúdo será nulo ou vazio. É possível inicializar uma variável juntamente à sua declaração:

```
cadeia nome = "Fulano"
```

Mas podemos também declarar uma variável e inicializá-la com um valor lido:

```
real preco
leia(preco)
```

O comando `leia()` utilizado no exemplo acima será abordado na próxima seção.

Antes de prosseguirmos, lembre-se que você pode declarar quantas variáveis quiser e de diversos tipos diferentes em um mesmo programa, por exemplo:

```
cadeia nome, sobrenome, apelido
real peso, altura
inteiro idade
```

### 6.2\. Comandos de entrada

Comandos de entrada são os responsáveis por receber uma informação do usuário. Ex.: leia, escute, ouça, receba.

```
leia(nome)
```

Quando se trata de linguagens de programação, os comandos costumam ter um par de parênteses logo após seu nome, onde serão informadas opções para sua execução. Neste exemplo, o valor lido pelo comando `leia()` é armazenado na variável `nome`.

### 6.3\. Comandos de saída

Comandos de saída são os responsáveis por enviar uma informação ao usuário. Ex.: escreva, imprima, mostre, exiba.

```
escreva(“Olá, mundo!”)
```

Neste exemplo, o comando `escreva()` irá exibir na tela o texto `Olá, mundo!`.

### 6.4. Um básico exemplo de entrada, processamento e saída

Neste exemplo, iremos declarar três variáveis: `a`, `b` e `c`, todas do tipo `inteiro`. Faremos a leitura de dois valores e os armazenaremos nas variáveis `a` e `b`. A variável `c` receberá a soma de `a` e `b`. Por fim, escreveremos o valor contido em `c`.

```
inteiro a, b, c
leia(a)
leia(b)
c = a + b
escreva(c)
```

Perceba que as últimas duas linhas do exemplo acima poderiam ser substituídas por:

```
escreva(a + b + c)
```

### 6.5. Dando mais sentido ao seu código

Pense numa situação em que você precise escrever um programa em dupla, juntamente com um de seus colegas de classe. Fica combinado que você escreverá a primeira parte do programa e seu colega completará a solução a partir daí. No entanto, devido ao pequeno prazo disponível, você não poderá explicar ao seu colega pessoalmente como fez para chegar até aquele ponto da solução.

Podemos acreditar que, muito provavelmente, seu colega terá dificuldades em compreender seu código para, então, conseguir prosseguir com a solução do problema.

Mas, e se você pudesse escrever algo mais dentro do seu código para orientar seu colega sem que isso atrapalhasse o funcionamento do seu programa? Isso é possível com o uso de **comentários**.

Através de comentários, você pode escrever qualquer coisa dentro do seu código sem que isso afete o funcionamento do seu programa. Para escrever um comentário, apenas insira `//` e escreva seu comentário. Exemplo:

```
inteiro x = 50
// Isto é um comentário de uma única linha
escreva(x)
```

Às vezes utilizamos comentários também para **suprimir** uma ou mais linhas de código de um programa para que elas não sejam executadas:

```
inteiro x = 10, y = 20
escreva(x)
// escreva(y)
// Veja que só a variável x será escrita, pois a linha que deveria escrever y foi marcada como um comentário
```

Alguns comentários podem ser mais longos e ocupar várias linhas de código. Neste caso, a primeira linha comentada deverá ser iniciada com `/*` e a última finalizada com `*/`. Exemplo:

```
inteiro z = 30
/* Este comentário
foi um pouco
mais longe */
escreva(z)
```

## 7. Estruturas de decisão: escolha um caminho

Na programação, há momentos em que precisamos fazer decisões, definir caminhos diferentes para situações diferentes, e é por isso que existem as **estruturas de decisão**.

As duas estruturas de decisão presentes na maioria das linguagens de programação são o se/senao (if/else, em inglês) e o escolha/caso (switch/case, em inglês).

As estruturas de decisão são peça fundamental na estruturação dos algoritmos utilizados nos sistemas que utilizamos diariamente. Por exemplo, pense em quando você entra com seu e-mail e senha para realizar login em uma rede social. Observe que no momento em que você clica no botão Entrar, duas situações são possíveis: seu login pode ser aceito e você entrará na rede social, ou a página indicará que seu e-mail e/ou senha estão incorretos. Para decidir qual das duas ações realizar, o sistema certamente fez uso de uma estrutura de decisão.

### 7.1. Se

A estrutura `se` é utilizada na maioria dos casos em que se faz necessário decidir que ação será tomada.

Para que você compreenda como funciona a estrutura `se`, imagine a seguinte situação: após lermos um número inteiro qualquer, se este número for par, deveremos exibir uma mensagem informando que ele é par. Ex.:

```
inteiro numero
leia(numero)
se(numero % 2 == 0) {
    escreva("O número lido é par.")
}
```

A partir da terceira linha do código acima, começamos a utilizar a estrutura de decisão `se`. Observe que ela é constituída da palavra "se" seguida de um par de parênteses. Dentro dos parênteses deve haver uma expressão lógica, ou seja, uma expressão que possa ser avaliada como `verdadeiro` ou `falso`. Quando a expressão entre parênteses é igual a `verdadeiro`, o código entre as chaves da estrutura é executado. Se o resultado da expressão for `falso`, o código entre as chaves é simplesmente ignorado.

Neste exemplo, a expressão avaliada é `numero % 2 == 0`. Considerando que a variável `numero` contenha mesmo um número par, como 4, sabemos que o resultado da expressão `numero % 2` será igual a 0, pois ao se dividir 4 por 2, o resto (ou módulo) é 0, logo a expressão retornará o valor `verdadeiro`. Observe:

```
4 % 2 == 0
0 == 0
verdadeiro
```

Se o valor da variável `numero` for ímpar, o resto da sua divisão por 2 será 1, o mesmo acontecerá com qualquer outro número ímpar, logo a expressão retornará o valor `falso`. Observe:

```
3 % 2 == 0
1 == 0
falso
```

### 7.2. Se/Senão

Nem sempre é suficiente apenas verificar se uma condição é atendida e executar determinada ação. Muitas vezes precisamos de uma segunda alternativa, um plano B.

Ainda conforme o exemplo abordado anteriormente, imagine que caso o número lido não seja par tenhamos que mostrar uma mensagem também informando que o número é ímpar. Acompanhe o exemplo:

```
inteiro numero
leia(numero)
se(numero % 2 == 0) {
    escreva("O número lido é par.")
} senao {
    escreva("O número lido é ímpar.")
}
```

Observe que na quinta linha adicionamos a palavra `senao`, seguida de um par de chaves. Neste caso, o código entre as chaves só será executado se a expressão verificada no bloco `se` não for igual a `verdadeiro`, ou simplesmente for igual a `falso`.

### 7.3. Se/Senão/Se

Mas o que fazer quando temos mais de duas alternativas?

Para responder a essa pergunta, vamos pensar no seguinte problema: após ler um número inteiro, precisamos informar ao usuário se este número é negativo, nulo (0) ou positivo. Podemos fazer isso da seguinte forma:

```
inteiro numero
leia(numero)
se(numero < 1) {
    escreva("O número lido é negativo.")
} senao se(numero > 1){
    escreva("O número lido é positivo.")
} senao {
    escreva("O número lido é nulo.")
}
```

Observe que neste caso foram testadas duas condições: `numero < 1` e `numero > 1`. A segunda condição segue acompanhando o primeiro `senao`, indicando que esta condição só deverá ser verificada caso a primeira não seja verdadeira. Por fim, considerando que nenhuma das duas condições seja verdadeira, o código após o segundo `senao` poderá ser executado.

Mais uma vez:
- Se `numero < 1` for `verdadeiro`, o código `escreva("O número lido é negativo.")` será executado.
- Se `numero < 1` for `falso` e `numero > 1` for `verdadeiro`, o código `escreva("O número lido é positivo.")` será executado.
- Se `numero < 1` for `falso` e `numero > 1` for `falso`, o código `escreva("O número lido é nulo.")` será executado.

Tenha em mente que a quantidade de testes que podem ser realizados em sequência é basicamente ilimitada, mas não é comum vermos estruturas de decisão exageradamente longas.

Para adquirir um maior domínio, teste os exemplos vistos, mas não pare por aí, crie seus próprios exemplos, teste condições compostas, como `idade > 18 e peso < 70`, estruturas com e sem um `senao`, com dois ou mais `senao se` até perceber que já está dominando o assunto.

### 7.2. Escolha/Caso

Em construção.

## 8. Estruturas de repetição: como evitar a fadiga

Quando programamos, algumas tarefas podem exigir esforços absurdamente repetitivos. Imagine uma situação em que seja necessário exibir uma lista numerada com 50 itens. Será que precisaríamos mesmo repetir o comando `escreva()` por 50 vezes?

A boa notícia é que alguém já pensou nisso antes. As linguagens de programação possuem estruturas que chamamos de **estruturas de repetição** ou de **laços de repetição**. Estas estruturas são utilizadas sempre que nos deparamos com tarefas que exijam que um procedimento se repita por várias vezes.

As três estruturas de repetição que abordaremos são: enquanto (while, em inglês), faca/enquanto (do/while, em inglês) e para (for, em inglês). Cada uma dessas estruturas é mais adequada em uma situação específica, mas o propósito de automatizar tarefas repetitivas permanece em todas elas.

Assim como nas estruturas de decisão, o funcionamento de uma estrutura de repetição é baseado em uma condição, que mais uma vez deverá ser representada através de uma expressão lógica.

A seguir, conheceremos cada uma das estruturas de repetição mais a fundo.

### 8.1. Enquanto

Imagine uma situação em que você precise repetir determinada tarefa enquanto uma certa condição for verdadeira, por exemplo:

>> Enquanto um for igual a um, escreva: um é igual a um.

Essa mesma situação pode ser descrita em código, utilizando Portugol, da seguinte forma:

```
enquanto(1 == 1)
{
    escreva("um é igual a um.")
}
```

Neste exemplo, enquanto a condição `1 == 1` for avaliada como verdadeira, a expressão `escreva("um é igual a um.")` será executada. Pense nisso como um ciclo: avaliamos a condição, se ela for verdadeira, o código é executado, depois tudo se repete novamente.

Se você testou o código acima, deve ter percebido que ele gerou um **loop infinito**, que é como chamamos os laços de repetição intermináveis. O motivo de esse laço de repetição ser interminável é bastante óbvio, pois sabemos que 1 será sempre igual a 1, logo a condição sempre será verdadeira.

Quando a condição é avaliada como falsa, o código entre chaves não é executado e o programa segue para após a estrutura de repetição.

```
enquanto(esta condição for verdadeira)
{
    este código será executado
    ...e a condição será verificada novamente
}
se a condição for falsa, o código continuará daqui
```

Em muitos dos casos em que utilizamos laços de repetição, nós trabalhos com números inteiros. Considere, por exemplo, uma situação em que seja necessário imprimir todos os números inteiros de 1 a 10. Em casos como este, utilizamos variáveis do tipo inteiro que possam ter seu valor alterado progressivamente. A estas variáveis damos o nome de **contadoras**:

```
inteiro x = 1
enquanto(x <= 10)
{
    escreva(x)
    x = x + 1
}
```

No exemplo acima, a variável `x` assume o papel de contadora, pois é utilizada como condição do laço de repetição e seu valor é **incrementado** a cada repetição. A variável é inicializada com o valor `1` e definimos que enquanto o valor nela contido for menor ou igual a `10`, a seguinte tarefa deve ser executada: escreve-se o valor de `x` e adiciona-se `1` ao valor atual de `x`.

Ao término desse programa, o valor de `x` será igual a `10` ou igual a `11`? Perceba que em algum momento nessa estrutura de repetição, o valor de `x` atingirá `10`, a condição entre parênteses será avaliada como verdadeira, o valor de `x` será mostrado e incrementado, ou seja, `x` passará a ser igual a `11`. A partir deste ponto, a condição `x <= 10` voltará a ser avaliada e, desta vez, seu resultado será `falso`, pois `x` é igual a `11`, logo não é nem menor nem igual a `10`. Com isto, o laço de repetição será interrompido e o valor de `x`, que agora é igual a `11`, não será mais mostrado.

Se precisarmos realizar o caminho contrário, ou seja, imprimir todos os números inteiros de 10 a 1 (em ordem decrescente), o seguinte código seria suficiente:

```
inteiro x = 10
enquanto(x >= 1)
{
    escreva(x)
    x = x - 1
}
```

Perceba que, neste exemplo, o valor de `x` é **decrementado**, ou seja, subtraímos `1` do valor de `x` a cada repetição. A condição verificada também é diferente: desta vez, verificamos a cada repetição se o valor de `x` é maior ou igual a `1`.

De forma bastante resumida, podemos descrever a estrutura `enquanto() { }` da seguinte forma:

1. A condição é testada
2. Se a condição for avaliada como verdadeira, o código entre chaves é executado, retorna-se ao passo 1
3. Se a condição for avaliada como falsa, segue-se ao passo 4
4. A estrutura é finalizada

### 8.2. Faça/Enquanto

A segunda estrutura de repetição que iremos abordar funciona de forma muito semelhante à primeira, com uma pequena diferença: a condição só é verificada após a primeira execução do código. Observe o exemplo:

>> Escreva: um é igual a um. Enquanto um for igual a um, repita.

Essa mesma situação pode ser descrita em código, utilizando Portugol, da seguinte forma:

```
faca
{
    escreva("um é igual a um.")
}
enquanto(1 == 1)
```

De forma bastante resumida, podemos descrever a estrutura `faca { } enquanto()` da seguinte forma:

1. O código entre chaves é executado
2. A condição é testada
3. Se a condição for avaliada como verdadeira, retorna-se ao passo 1
4. Se a condição for avaliada como falsa, segue-se ao passo 5
5. A estrutura é finalizada

#### * Bônus

Se você ainda não conseguiu compreender a diferença entre `enquanto` e `faca enquanto`, reflita nas seguintes situações:

Enquanto:
> Mariana pede a Felipe que vá ao mercado e lhe diz: Felipe, se os tomates estiverem bons, pegue um. Enquanto houver tomates bons, continue pegando tomates. Se não houver mais tomates bons, pare de pegar os tomates.

Faça/Enquanto:
> Mariana pede a Felipe que vá ao mercado e lhe diz: Felipe, pegue um tomate. Enquanto houver tomates bons, continue pegando tomates. Se não houver mais tomates bons, pare de pegar os tomates.

![alt text](imagens/tomato.jpg "Tomate")

### 8.3. Para

A última estrutura de repetição que iremos abordar tem um comportamento bastante semelhante ao das anteriores, porém, tem uma finalidade muito específica: a estrutura de decisão `para` é a mais adequada em situações em que o número de repetições a serem executadas já é conhecido.

Observe como faríamos para imprimir os números inteiros de 1 a 1000 utilizando `para`:

```
para(inteiro x = 1; x <= 1000; x++)
{
    escreva(x)
}
```

Você pode ter a impressão de que a condição entre parênteses ficou maior, mas não é exatamente isso o que acontece. Ao utilizarmos a estrutura `para`, temos acesso a três regras, separadas por ponto e vírgula, que definirão como a estrutura será executada. A estas regras damos o nome de **parâmetros** ou **argumentos**.

1. O primeiro parâmetro é um espaço disponibilizado para a declaração e inicialização de variáveis que serão utilizadas apenas dentro desta estrutura `para`. Observe que no exemplo acima, nós declaramos e inicializamos a variável `x` com o valor `1`. A variável `x` será nossa contadora e, por vezes, também poderá ser chamada de **variável de controle**.
2. O segundo parâmetro é referente à condição que será verificada a cada repetição. Enquanto a expressão informada for avaliada como verdadeira, o código continuará a ser repetido. No exemplo acima, definimos que o código será repetido enquanto o valor de `x` for menor ou igual a `1000`.
3. O terceiro e último parâmetro é destinado à definição da alteração que a variável de controle irá sofrer a cada repetição. Geralmente, definimos nesta posição uma expressão de incremento ou de decremento da variável de controle. Em nosso exemplo, a variável `x` é incrementada em `1` a cada repetição.

De maneira resumida, podemos dizer que: considerando a(s) variável(eis) de controle definida(s), enquanto a condição informada for verdadeira, o valor da(s) variável(eis) de controle será alterado e o código entre chaves será executado.

#### * Bônus

Você deve ter notado em nossa estrutura de repetição `para` o uso da expressão `x++`. Os operadores `++` podem ser utilizados com qualquer variável numérica, seja inteira ou real, quando se deseja incrementar seu valor em `1`.

Para decrementar o valor de `x` em `1`, poderíamos ter feito `x--`.

Observe que isto pode ser utilizado em qualquer momento no código, tanto na estrutura `para` quanto em qualquer outra estrutura de repetição ou mesmo fora de uma estrutura de repetição.

Os seguintes métodos de incremento são equivalentes:

```
x = x + 1
x += 1
x++
```

Qualquer um dos métodos acima fará com que o valor contido em `x` seja incrementado em `1`, ou seja: se o valor de `x` for `5`, por exemplo, `x++` fará com que `x` passe a valer `6`.

O mesmo é válido para decremento:

```
x = x - 1
x -= 1
x--
```

Caso seja necessário incrementar ou decrementar o valor de uma variável em mais que `1`, os operadores `++` ou `--` não poderão ajudar. Em casos como estes, apenas os dois primeiros métodos mostrados irão funcionar. Exemplo:

```
// Incremento
x = x + 3
x += 3

// Decremento
y = y - 5
y -= 5
```

## 9. Referências Bibliográficas

- LOPES, Anita. GARCIA, Guto. **Introdução à programação – 500 algoritmos resolvidos**. Rio de Janeiro: Elsevier, 2002 - 15ª Tiragem.

## Lista 1 - Expressões, entrada e saída de dados

1. Leia dois números inteiros e escreva o resultado de sua soma.
2. Leia dois números inteiros e escreva o resultado de sua subtração.
3. Leia dois números inteiros e escreva o resultado de sua multiplicação.
4. Leia dois números inteiros (`a` e `b`) e escreva o resultado da divisão `a / b`.
5. Leia dois números inteiros (`a` e `b`) e escreva o resultado do resto da divisão `a % b`.
6. Leia dois números reais e escreva o resultado de sua soma.
7. Leia o nome de uma pessoa e escreva uma frase de saudação, como: `Olá, Fulano`.
8. A média aritmética de dois ou mais termos é o quociente do resultado da divisão da soma dos números dados pela quantidade de números somados. Elabore um algoritmo que leia as 4 notas de um aluno e escreva sua média aritmética.
9. A autonomia de um veículo é baseada em quantos quilômetros ele consegue percorrer a cada litro de combustível consumido. Por exemplo, é comum afirmar que tal carro é capaz de fazer 15 quilômetros por litro de combustível. Com base nisso, elabore um algoritmo que leia uma distância percorrida em quilômetros e uma quantidade de litros de combustível consumidos, e informe quantos quilômetros este veículo pode percorrer com cada litro.
10. A velocidade média de um veículo pode ser calculada se tivermos os seguintes valores: a distância percorrida e o tempo gasto para percorrer esta distância. Com base nisso, elabore um algoritmo que leia uma distância percorrida em quilômetros e o tempo gasto em horas, e informe a velocidade média desse veículo.
11. Alguns países de língua inglesa, como os EUA, utilizam da unidade de medida grau Fahrenheit como escala de temperatura. Para converter uma temperatura de Celsius para Fahrenheit, podemos aplicar a fórmula `F=(9*C+160)/5` ou a fórmula `F=C*1.8+32`, onde F é a temperatura em Fahrenheit e C a temperatura em Celsius. Elabore um algoritmo que leia uma temperatura em graus Celsius e a escreva convertida em graus Fahrenheit.
12. Para auxiliar uma loja que deseja parcelar o valor das compras de seus clientes, elabore um algoritmo que leia o valor de uma compra e o número de prestações desejadas, e escreva o valor das prestações.
13. No comércio, os preços dos produtos geralmente são definidos com base em uma margem percentual de lucro. Considere um produto adquirido por uma loja pelo valor de R$ 100,00\. Se esta loja aplicar a este produto um percentual de 15% de lucro, o produto será revendido pelo valor de R$ 115,00\. Elabore um algoritmo que leia o valor de compra de um produto e o percentual de lucro desejado, e escreva o valor de revenda deste produto.
14. Você foi encarregado de realizar uma pesquisa sobre Inclusão Digital. A sua pesquisa deverá apresentar o percentual de alunos da sua escola que possuem acesso à internet. Para isso, elabore um algoritmo que leia o número total de alunos da sua escola e o número de alunos que possuem acesso à internet, por fim, com base nestes dados, escreva o percentual de alunos com acesso à internet. Ex.: Em uma escola com 200 alunos, apenas 50 alunos possuem acesso à internet, o que equivale a 25% destes 200 alunos.
15. Em uma pequena loja de eletrônica são vendidos `resistores`, `diodos` e `transistores`. Seus preços são `R$ 0.70`, `R$ 0.80` e `R$ 0.95`, respectivamente. Têm-se os preços unitários de cada tipo de peça e sabe-se que sobre estes preços incidem descontos de `5%` para `resistores`, `6%` para `diodos` e `9%` para `transistores`. Elabore um programa que leia o nome do cliente e as quantidades de cada item comprado; e escreva o valor total de desconto e o valor líquido a ser pago pela compra.

## Lista 2 - Estruturas de decisão: Se/Senão

1. Leia um número inteiro e informe se este número é par ou ímpar.
2. Leia a idade de uma pessoa e informe se ela já chegou à maioridade. Se ela ainda não chegou, informe quantos anos faltam para a maioridade.
3. Construa um algoritmo que leia um número inteiro A e um número inteiro B. Verifique qual dos dois números é maior e o escreva.
4. Considerando uma pista em que a velocidade máxima permitida é de 110 km/h, leia a velocidade de um veículo e informe se ele excedeu ou não a velocidade máxima permitida.
5. Considerando que a temperatura média ideal do corpo humano varia entre 36° C e 36,7° C, elabore um algritmo que, dada uma temperatura lida, informe se esta pessoa está com febre.
6. Complemente o algoritmo anterior, adicionando a ele a capacidade de informar se a pessoa está com hipotermia (abaixo da temperatura média ideal); dentro da temperatura média ideal ou com febre.
7. Elabore um algoritmo que leia um número inteiro e informe se este número é um múltiplo de 7.
8. Leia um número inteiro e informe se este número é par e também divisível por 3.
9. Para auxiliar um cliente a escolher o produto mais barato em um conjunto de 3 produtos, crie um programa que leia os preços de 3 produtos e informe qual deles é o mais barato.
10. Construa um programa que leia um caractere e informe se este caractere é uma vogal.
11. Leia dois números inteiros `x` e `y`, e informe se `x` é divisível por `y`.
12. Considerando que no Brasil é possível votar a partir dos 16 anos de idade, leia o ano de nascimento de uma pessoa e informe se ela poderá votar no ano atual. Ignore mês e dia de nascimento.
13. Considerando que o ano possui 12 meses, leia um número inteiro de 1 a 12 e informe o mês que corresponde a este número.
14. Leia dois números inteiros `x` e `y` e escreva dentre as seguintes hipóteses a verdadeira: 1\. `x` e `y` são pares; 2\. `x` e `y` são ímpares; 3\. `x` é par e `y` é ímpar; 4\. `x` é ímpar e `y` é par.
15. Para auxiliar a definir os períodos mais quente e mais frio do dia, elabore um algortimo que leia a temperatura do período matutino, a temperatura do período vespertino e a temperatura do período noturno, ao fim escreva qual destes períodos foi o mais frio e qual foi o mais quente.
16. Construa um algoritmo que leia as medidas dos lados de um triângulo e informe se este triângulo é equilátero, isósceles ou escaleno.
17. Construa um algoritmo que leia um número real e, se ele for maior do que 5, então escreva a metade deste número. Ex.: se leio o número 12, 12 é maior que 5; a metade de 12 é 6; devo escrever 6.
18. Construa um algoritmo que leia um número inteiro e, se ele for positivo, escreva uma mensagem que informe se este número é ou não divisível por 2.
19. Construa um algoritmo que leia dois números inteiros diferentes e escreva-os em ordem crescente.
20. Construa um algoritmo que leia três números inteiros e escreva-os em ordem decrescente.
21. Crie um algoritmo que leia dois números inteiros e escreva uma mensagem dizendo se estes números são iguais ou diferentes.
22. O IMC (Índice de Massa Corporal) é uma unidade de medida internacional usada para calcular se uma pessoa está no seu peso ideal. A fórmula mais genérica de cálculo de IMC é `imc = peso / altura * altura`, onde o peso é dado em quilos e a altura em metros. Há uma tabela que define uma classificação para cada faixa de IMC. Segundo esta tabela, pessoas com IMC menor ou igual a 18.5 estão abaixo do peso; pessoas com IMC maior que 18.5 e menor que 25 estão no peso ideal; já as pessoas com IMC maior ou igual a 25 estão acima do peso. Elabore um algoritmo que leia peso e altura de uma pessoa, informe seu IMC e também se ela está abaixo do peso, no peso ideal ou acima do peso.

## Lista 3 - Estruturas de decisão: Escolha/Caso

1. Elabore um programa que leia uma letra e informe se esta letra é uma vogal ou uma consoante.
2. Elabore um programa que funcione como uma calculadora simples. Seu programa deverá começar mostrando uma mensagem de apresentação, depois solicitar que o usuário entre com dois números reais (`a` e `b`) e finalmente ler os dois números reais digitados.  Logo após, o programa deverá solicitar ao usuário que escolha uma das seguintes opções: somar, subtrair, multiplicar ou dividir. Com base na escolha do usuário, exiba o resultado da operação escolhida envolvendo `a` e `b`.
3. Considerando que o ano possui 12 meses, leia um número inteiro entre 1 e 12 e, com o uso da estrutura de controle escolha/caso, informe o nome do mês que corresponde a este número.
4. Verificar a quantidade de combustível que será gasta em uma viagem é de grande importância para o condutor. Considerando que um carro do tipo A é capaz de percorrer 12 quilômetros a cada litro de combustível gasto, um do tipo B percorre 9 quilômetros a cada litro e um do tipo C, 8 quilômetros por litro, elabore um programa que leia a distância a ser viajada e o tipo de carro, e com base nestes dados informe quantos litros de combustível serão gastos.
5. Construa um programa que funcione como um menu para uma lanchonete. Seu programa deverá iniciar mostrando o nome da sua lanchonete. Em seguida, seu programa deverá pedir o nome do usuário e, após lê-lo, exibir uma mensagem de boas vindas. Após isso, seu programa deverá mostrar as opções de lanches disponíveis e seus preços: mostre pelo menos 6 opções de lanches diferentes. Permita que o usuário escolha uma das opções de lanches e, após a escolha, mostre a ele uma mensagem informando a opção que ele escolheu e quanto seu pedido irá custar. Lembre-se de avisar ao usuário caso ele escolha uma opção inexistente.
6. Construa um programa que leia a primeira letra do mês de nascimento de uma pessoa e informe em quais meses essa pessoa pode ter nascido. Caso não exista um mês que comece com a letra lida, informe ao usuário que ele se enganou.

![alt text](imagens/meses.png "Meses")

## Lista 4 - Laços de Repetição: Enquanto e Faça/Enquanto

1. Elabore um algoritmo que escreva todos os números inteiros de 1 a 100.
2. Elabore um algoritmo que escreva apenas os números pares de 1 a 100.
3. Elabore um algoritmo que escreva apenas os números ímpares de 1 a 100.
4. Elabore um algoritmo que escreva todos os números inteiros de 200 a 400.
5. Elabore um algoritmo que escreva apenas os números pares de 300 a 600.
6. Elabore um algoritmo que escreva apenas os números ímpares de 750 a 1500.
7. Construa um programa que leia um número inteiro e escreva todos os números inteiros de 1 até o número lido.
8. Construa um programa que leia um número inteiro, verifique se ele é par ou ímpar. Se o número for ímpar, escreva todos os números ímpares menores que ele em ordem crescente. Se o número for par, escreva todos os números pares menores que ele em ordem crescente.
9. Repita a questão anterior, desta vez imprimindo os números em ordem decrescente, desde o número lido.
10. Construa um programa que comece lendo um número inteiro qualquer. Este número será chamado de `piso`. Após isso, seu programa deverá ler um outro número inteiro (que poderá ser chamado de `proximo`) enquanto `proximo` for maior ou igual a `piso`.
11. Elabore um algoritmo que leia dois números inteiros diferentes: `ini` e `fim`, sendo que `ini` deve ser menor que `fim`. Escreva em ordem crescente todos os números inteiros entre `ini` e `fim`, inclusive eles mesmos.
12. Repita a questão anterior, desta vez presumindo que `ini` pode ou não ser maior que `fim`. Se `ini` for maior que `fim`, siga a ordem decrescente.
13. Construa um programa que repita a tarefa de ler um número inteiro, enquanto o número lido for maior que 1. Ao término das repetições, escreva o resultado da soma de todos os números lidos.
14. Construa um algoritmo que leia dois números inteiros diferentes: `ini` e `fim`, sendo que `ini` deve ser menor que `fim`. Em seguida, escreva o resultado da soma de todos os números inteiros entre `ini` e `fim`, contando com eles mesmos.
15. Construa um programa que calcule as médias aritméticas de todos os alunos de uma turma. Seu programa deverá funcionar da seguinte maneira: leia o nome do aluno; leia as notas dos 4 bimestres; mostre a média aritmética do aluno; pergunte se o usuário deseja continuar; se o usuário desejar continuar, repita todo o processo, senão, pare.

## Lista 5 - Laços de Repetição: Para

1. Elabore um algoritmo que escreva todos os números inteiros de 1 a 100.
2. Elabore um algoritmo que escreva apenas os números pares de 1 a 100.
3. Elabore um algoritmo que escreva apenas os números ímpares de 1 a 100.
4. Elabore um algoritmo que escreva todos os números inteiros de 200 a 400.
5. Elabore um algoritmo que escreva apenas os números pares de 300 a 600.
6. Elabore um algoritmo que escreva apenas os números ímpares de 750 a 1500.
7. Elabore um algoritmo que leia as quatro notas de um aluno e, ao fim, mostre sua média aritmética.
