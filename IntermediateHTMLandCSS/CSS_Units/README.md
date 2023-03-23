# [CSS Units](https://www.theodinproject.com/lessons/node-path-intermediate-html-and-css-css-units)

Essa parte fala sobre as [unidades do CSS](https://www.theodinproject.com/lessons/node-path-intermediate-html-and-css-css-units) absolutas e relativas.

- O que eu achei mais interessante foi esse [artigo do CSS Tricks](https://css-tricks.com/fun-viewport-units/) sobre as medidas de viewport. Dá pra alcançar uns resultados interessantes de posicionamento usando **vw** ou **vh**.
	- Vale mencionar esse outro [artigo do Chrome Developers](https://developer.chrome.com/blog/url-bar-resizing/) sobre a mudança do viewport no navegador para Android. As versões mais recentes não consideram a barra da URL como parte do viewport, portanto, usar um **100vh** vai além do limite da tela.

---
Aprendi duas funções novas para usar no console do JS e lembrei de outras que já tinha visto:
```js
// Põe em tela cheia
document.documentElement.webkitRequestFullscreen()

// Sai da tela cheia
document.webkitExitFullscreen()

// Redireciona para outra página (pode ser um arquivo html ou um link)
window.location.href = "caminho/do/arquivo.html" 
window.location.href = "https://www.google.com"

// Volta para a página anterior
window.history.back()
```

- Nos arquivos **index.html** e **pagina2.html** eu fiz um exemplo básico pra essas funções acima. Além disso, testei o exemplo do CSS Tricks com **``body { height: 100vh; display: grid; }``**.
- Pra esse teste eu usei o [Live Server (Five Server)](https://marketplace.visualstudio.com/items?itemName=yandeu.five-server) do VS Code pra rodar o servidor local (no PC) e Lan (no celular), além do [GitHub Copilot](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot) pra ajudar na digitação e testar como ele está no momento.

Uma outra dica, mas de CSS agora. Já viu que quando tem algo clicável no celular (como um link ou botão) ele mostra uma sobreposição azul quando você clica? Pra tirar isso, basta adicionar: 
```css
button, a {
	-webkit-tap-highlight-color: transparent;
}
```
no CSS que ela some. Claro que isso só funciona no Chrome e derivados, mas é uma boa pra tirar aquele efeito de clique que fica meio feio.

Para ver os testes, acesse:
- [index.html](https://brianmath.github.io/TheOdinProject/IntermediateHTMLandCSS/CSS_Units/index.html) - comece por aqui
- [pagina2.html](https://brianmath.github.io/TheOdinProject/IntermediateHTMLandCSS/CSS_Units/pagina2.html).