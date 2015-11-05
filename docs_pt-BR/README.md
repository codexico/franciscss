> Um conjunto de técnicas para escrever CSS mais rapidamente e evitar código de difícil manutenção.


## Introdução

É muito comum pegar CSS legado com milhares de linhas e tudo bagunçado, você precisa trocar a posição de um título e acaba tendo que escrever algo assim:

```css
body #main.page-layout2 .content #artigoSuper h2#title.nsb.l  { /* */ }
```
**Quem nunca né?**

> O que é aquela classe `.nsb`? A chance é grande do `.l` ser float:left ...

**Pois é, que tal se fosse assim:**

```css
.article-title { /* */ }
```


# Modularizar
### Dividir para conquistar

Imagine o html como pequenos retângulos, do menor para o maior.

Vamos dividir em **modules**, **elements**, **states** e **variations**.

* Se é uma parte dentro de outra, então é um **element**.
  * Ex: input de um form
* Se é uma parte independente, será um **module**.
  * Ex: um blog post
* Parece só layout, é um **module**.
  * Ex: grid
* Muda com hover ou algo assim, é um **state** de um elemento ou módulo.
  * Ex: input com erro
* Parece com outro módulo ou elemento, é uma **variation**.
  * Ex: botões enviar e cancelar


> Você devia escrever seu código como se quem fosse pegar para dar manutenção fosse um psicopata que sabe onde você mora.

> > Eu já havia escutado uma versão dessa frase, aí aconteceu comigo, tive um colega de trabalho que estava sempre com uma aba aberta com algum site sobre armas. É melhor codar direitinho, vai que esse cara pega seu código para fazer alguma alteração :o

Vamos começar com os módulos.
[Continuar →](docs_pt-BR/components.md)


# Table of contents

- [rscss](../README.md)
- **Components**
  - [About components](components.md)
  - [Elements](elements.md)
  - [Variants](variants.md)
  - [Nested components](nested-components.md)
  - [Layouts](layouts.md)
  - [Helpers](helpers.md)
- **Structure**
  - [CSS Structure](css-structure.md)
- **Notes**
  - [Pitfalls](pitfalls.md)
  - [Apprehensions](apprehensions.md)
  - [Other resources](other-resources.md)
- [Summary](summary.md)
