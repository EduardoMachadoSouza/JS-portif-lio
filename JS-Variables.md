# JS Variables

Em JavaScript, você pode declarar variáveis usando três palavras-chave diferentes: `var`, `let` e `const`. Cada uma delas tem características distintas relacionadas ao escopo e à mutabilidade da variável.

### `var` (Declaração de Variável Antiga)

- Variáveis declaradas com `var` têm escopo de função ou escopo global.
- Elas podem ser **redeclaradas** no mesmo escopo.
- Variáveis `var` são iniciadas (hoisted), o que significa que a declaração é movida para o topo do escopo, mas a inicialização permanece no lugar.
- Não é recomendado o uso de `var` em código moderno devido a problemas de escopo e previsibilidade.

### `let` (Declaração de Variável Moderna)

- Variáveis declaradas com `let` têm **escopo de bloco**, o que significa que são limitadas ao bloco mais próximo em que foram declaradas.
- Elas não podem ser redeclaradas no mesmo escopo.
- As variáveis `let` não são iniciadas no mesmo grau que as variáveis `var`. Elas são iniciadas apenas no sentido de que a declaração é movida para o topo do bloco.

### `const` (Declaração de Constante)

- Variáveis declaradas com `const` também têm escopo de bloco.
- Elas não podem ser reatribuídas após a inicialização. No entanto, objetos e arrays declarados com `const` podem ter seus valores internos modificados.
- Como `const` **não permite a reatribuição**, é uma boa escolha para declarar variáveis que **não devem ser alteradas** após a inicialização.

A prática recomendada é usar `let` para a **maioria** das suas variáveis, a menos que você saiba que uma variável não deve ser reatribuída, nesse caso, você deve usar `const`. O uso de `var` deve ser **evitado** em **código moderno** devido a **problemas de escopo e redeclaração**.