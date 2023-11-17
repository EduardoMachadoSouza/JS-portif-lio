
### Operadores aritméticos

|Operador|Descrição|
|---|---|
|+|Adição|
|-|Subtração|
|\*|Multiplicação|
|\*\*|Potenciação (ES2016)|
|\/|Divisão|
|\%|módulo (resto da divisão)|
|\+\+|Incrementação|
|\-\-|Decrementação|
|\=|Igual|

### Operadores de Atribuição

|Operador|Exemplo|Mesma coisa que|
|---|---|---|
|=|x = y|x = y|
|+=|x += y|x = x + y|
|-=|x -= y|x = x - y|
|\*=|x \*= y|x = x \* y|
|\/=|x \/= y|x = x \/ y|
|\%=|x \%= y|x = x \% y|
|\*\*=|x \*\*= y|x = x \*\* y|

### Operadores de comparação

| Operador | Descrição |
| --- | --- |
| == | igual |
| === | igualdade estrita |
| != | diferente |
| !== | diferença estrita |
| > | maior que |
| < | menor que |
| >= | maior ou igual a |
| <= | menor ou igual a |
| ? | operador ternário |

### Operadores lógicos

|Operador|Descrição|
|---|---|
|&&|E|
|\|\||Ou|
|!|Não|

### Operadores relacionais

|Operador|Descrição|
|---|---|
|typeof|Retorna um tipo de variável|
|instanceof|Retorna verdadeiro se o objeto especificado for do tipo de objeto especificado|

### Operadores bit a bit

|Operador|Expressão|Descrição|
|---|---|---|
|E|a & b|Retorna um 1 para cada posição em que os bits da posição correspondente de ambos operandos sejam uns.|
|Ou|a \| b|
|Ou ou|a ^ b|Retorna um 0 para cada posição em que os bits da posição correspondente são os mesmos [Retorna um 1 para cada posição em que os bits da posição correspondente sejam diferentes.]|
|Não|~ a|Inverte os bits do operando.|
|Deslocamento à esquerda|a << b|Desloca a em representação binária b bits à esquerda, preenchendo com zeros à direita.|
|Deslocamento à direita com propagação de sinal|a >> b|Desloca a em representação binária b bits à direita, descartando bits excedentes.|
|Deslocamento à direita com preenchimento zero|a >>> b|Desloca a em representação binária b bits à direita, descartando bits excedentes e preenchendo com zeros à esquerda.|

### Precedência dos Operadores

| Tipo de operador | Operadores individuais |
| --- | --- |
| membro | . [] |
| chamada / criação de instância | () new |
| negação / incremento | ! ~ - + ++ -- typeof void delete |
| multiplicação / divisão / resto ou módulo | * / % |
| adição / subtração | + - |
| deslocamento bit a bit | << >> >>> |
| relacional | < <= > >= no instanceof |
| igualdade | == != === \!\=\= |
| E bit a bit | & |
| OU exclusivo bit a bit | ^ |
| OU bit a bit | \| |
| E lógico | && |
| OU lógico | \|\| |
| condicional | ?: |
| vírgula | , |
| atribuição | = += -= *= /= %= <<= >>= >>>= &= ^= \|= |
