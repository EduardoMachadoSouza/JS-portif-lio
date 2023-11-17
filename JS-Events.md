
Eventos em JavaScript permitem que você responda a ações do usuário ou ações que ocorrem em elementos HTML, como cliques, movimentos do mouse, pressionamentos de teclas e muito mais. Eles são uma parte fundamental da programação web interativa.

### Eventos do DOM

- Eventos são acionados por ações do usuário (como clicar em um botão) ou ações no navegador (como carregar uma página).
- Os eventos podem ser associados a elementos HTML, como botões, imagens, formulários e outros elementos.

### Adicionando Manipuladores de Eventos

- Para responder a eventos, você pode adicionar manipuladores de eventos a elementos HTML usando JavaScript.
- O método mais comum para adicionar um manipulador de evento é o `addEventListener()`.

```js
let botao = document.getElementById("meuBotao");
botao.addEventListener("click", function() {
  alert("Botão clicado!");
});
```
### Tipos de Eventos Comuns

- Alguns tipos de eventos comuns incluem:
    - `click`: Acionado quando um elemento é clicado.
    - `mouseover` e `mouseout`: Acionados quando o cursor do mouse entra e sai de um elemento.
    - `keydown` e `keyup`: Acionados quando uma tecla do teclado é pressionada e liberada.
    - `submit`: Acionado quando um formulário é enviado.
    - `load`: Acionado quando uma página ou recurso é totalmente carregado.

### Objeto de Evento

- Quando um evento ocorre, um objeto de evento é criado com informações sobre o evento, como o tipo do evento, o elemento de destino e mais.
- Você pode acessar esse objeto em um manipulador de evento para obter informações sobre o evento.

```js
botao.addEventListener("click", function(event) {
  alert("Botão clicado no elemento: " + event.target.tagName);
});
```

### Remoção de Manipuladores de Eventos

- Você pode remover manipuladores de eventos usando o método `removeEventListener()`. Isso é útil quando você deseja parar de ouvir eventos em um elemento.

```js
botao.removeEventListener("click", minhaFuncao);
```

### Evento de Carregamento (Load)

- O evento `load` é usado para executar código após a página ou um recurso externo ser completamente carregado.

```js
window.addEventListener("load", function() {
  alert("A página foi carregada completamente.");
});
```

### Prevenção de Comportamento Padrão

- Em alguns casos, você pode querer evitar o comportamento padrão associado a um evento, como a submissão de um formulário.
- Para fazer isso, você pode chamar o método `preventDefault()` no objeto de evento.

```js
formulario.addEventListener("submit", function(event) {
  event.preventDefault(); // Impede a submissão padrão do formulário
});
```

Eventos são fundamentais para tornar as páginas web interativas e responsivas ao usuário. Eles permitem que você crie aplicações web dinâmicas e responsivas, onde ações do usuário desencadeiam respostas específicas.