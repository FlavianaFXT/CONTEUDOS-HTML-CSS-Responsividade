# CONTEUDOS-HTML-CSS-Responsividade


## INDICE

* [Entendendo sobre Responsividade](#Responsividade)
* [Tipos de imagem](#tiposdeimagem)
* [Unidade de medida](#unidadesdemedida)
* [Media Querie](#mediaquery)


### Entendendo a responsividade

![gif-responsivo](https://media.giphy.com/media/b2CD0Qrq2ulwY/giphy.gif)
Um **layout responsivo** é aquele que se "adapta" automaticamente aos dispositivos no qual ele está sendo visualizado, e é parte fundamental do conceito de **design responsivo**, que nada mais é do que a possibilidade de **adaptação fluida** de um site a diversos tamanhos de tela.

 #### Tipos de dispositivos: 
  - Notebooks 
  - Tablets
  - Desktops
  - Televisões

### Entendendo a responsividade

![responsivo-adaptativo](https://www.oficinadanet.com.br/imagens/post/13652/3038367-slide-s-1-9-gifs-that-explain-responsive-design-brilliantly-01responsive-vs-adaptive.gif)

O design responsivo expande de forma fluída, enquanto o adaptativo aguarda a tela terminar a expansão.
**Vantagens:**

* Usabilidade (design adaptado para diversos formatos);
* Manutenção (não precisa desenvolver outras versões);
* SEO Google (tudo em uma url só).

**Desvantagens:**

* Desenvolvimento apenas para os principais dispositivos do mercado;
* Versões antigas de navegadores que não reconhecem a linguagem de adapatação;
* Necessidade de uma pré construção da arquitetura do código e do layout.
* Um pouco mais demorado para carregar.

### Tipos de imagens 

* PNG: pouco compacta, mantém a qualidade da imagem, mas tem o tamanho elevado, sendo formatada por pixel.

* JPEG: mais compacta que PNG, tem baixa qualidade, tamanho menor  e não é possível usar transparência.

* GIF: efeito de animação, baixa qualidade.

* SVG: criados através de instruções ao computador, feito por cálculo. É mais leve que PNG.

Imagens em SVG tem seu uso mais comumente em  logotipo,  ícones, imagens mais simples. 
Nos demais casos, use sempre PNG, optando  por utilizar imagens com até 1500px.

### Unidades de medidas:

![gif-medidas](https://www.oficinadanet.com.br/imagens/post/13652/3038367-slide-s-2-9-gifs-that-explain-responsive-design-brilliantly-02relative-units-vs-static-units-1.gif)

####  Medidas absolutas

Essas são as mais comuns que vemos no dia a dia. São medidas que não estão referenciadas a qualquer outra unidade, ou seja, não dependem de um valor de referência.
Essas medidas são **estáticas** não mudam de acordo com as especificações do dispositivo.

_Quais são:_ 


  **pixels (px)**, points (pt), inches/polegadas (in), centímetro (cm), milímetro (mm) e paica (pc)

  
   ```
   * 96px = 1 in = 2,54cm = 25,4mm = 72pt = 6pc
   ```

Destas, pixel é a mais indicada e usada.

#### Medidas  relativas

Essas são as que normalmente não estamos habituados. Essas medidas são calculadas tendo como base uma outra unidade de medida pré-definida.

Devido ao fato de que essas medidas serem calculadas pelo browser baseando-se em outra unidade, elas tendem a ser bastantes **flexíveis**. Ou seja, podemos ter resultados diferentes de acordo com o tamanho de tela. 

_Quais são:_

* em

  **EM** vem de “ ephemeral”  e é uma unidade de **medida tipográfica**. Para entender sua aplicação, vamos utilizar o exemplo abaixo onde foi definido um tamanho de fonte no elemento `<div>`. O valor de **em** declarado em qualquer elemento-filho dentro de `<div>` será igual a: **o valor declarado no elemento-filho * o valor declarado no elemento pai**. 

  ```
    Nesse caso: **1.2(em) * 14px = 16.8px**
  ```

  ![unidade-em](./assets/img/unidade-em.jpg)

  Entretanto, o que acontece quando se tem um elemento com valor **em** dentro de outro elemento com valor **em** ?

HEAD
![unidade-em-aninhada](./assets/img/unidade-em-aninhada.jpg)

![unidade-em-aninhada](https://codepen.io/raissamartinsmenezes/pen/OJJXdzQ)


[Calculadora online: px para em](http://pxtoem.com/)

* rem

   O **REM** -  vem de “Root ephemeral”  e chega como sucessor do **EM** e ambos compartilham a mesma lógica de funcionamento, porém a forma de implementação é diferente. Enquanto o em está diretamente relacionado ao tamanho da fonte do elemento pai, o **rem** está relacionado com o tamanho da fonte do **elemento root (raiz)**. Embora sejam medidas tipográficas, **REM e EM** também podem ser utilizadas para outras finalidades, na atribuição de valores para margins e paddings por

![unidade-rem](./assets/img/unidade-rem.jpg)

Referência: [ Raissa Martins - Rem](https://codepen.io/raissamartinsmenezes/pen/LYYRZam)

[Calculadora online: px para rem](https://daniellamb.com/experiments/px-to-rem-calc/) 

* porcentagem %

Apesar de não ser uma unidade de medida, a porcentagem costuma ser bastante utilizada quando falamos de layout responsivo e fluido por conta de seu caráter adaptativo.

![porcentagem](./assets/img/porcentagem.jpg)
Referência: [ Raissa Martins - Porcentagem ](https://codepen.io/raissamartinsmenezes/pen/abbmJvY)

A porcentagem permite que criemos elementos que sempre vão se readaptar para ocupar a quantidade especificada.

![porcentagem-muda-tamanho](./assets/img/porcentagem-muda-tamanho.jpg)
Referência: [Raissa Martins - Porcentagem](https://codepen.io/raissamartinsmenezes/pen/abbmJvY)

**Note que a propriedade `width:` é relativa ao elemento-ancestral mais próximo.** 

* vh e vw

 Muitas técnicas de web design responsivo dependem muito de regras percentuais. **Mas e se fosse preciso usar a largura ou a altura da viewport ao invés da largura do elemento-pai?** Isso é exatamente o que as unidades vh e vw proporcionam.

 A medida vh é igual a **1/100** da altura da viewport. Então, por exemplo, se a altura do navegador é 900px, 1vh equivale a 9px e, analogamente, se a largura da viewport é 750px, 1vw equivale a 7.5px. Sendo assim, **1vw = 1% da largura da viewport e 1vh = 1% da altura da viewport**.


![vw-vh](./assets/img/vw-vh.jpg)

Vamos conferir o [exemplo 😊](./exemplos/exemplo-medidas-viewport.html)

* Outras unidades de medida

  **vmax e vmin:** [UNIDADES CSS RELATIVAS: VW, VH, VMAX, VMIN (CSS3)](https://www.youtube.com/watch?v=g__c-7M9Xzk&t=94s)

  **ex e ch:** [UNIDADES CSS RELATIVAS: %, REM, EM, CH, EX (CSS3)](https://www.youtube.com/watch?v=etM0JBeFbf8).




## LINKS DE ESTUDO


- [Guia de unidade de medida - Alura ](https://www.alura.com.br/artigos/guia-de-unidades-no-css)
- [Video explicativo - EM E REM ](https://www.youtube.com/watch?v=cnuZKcGLxiQ)
- [Video explicativo com exemplos - unidades relativas ](https://www.youtube.com/watch?v=etM0JBeFbf8)
- [Mais sobre unidades | W3 Schools ](https://www.w3schools.com/css/css_units.asp#)
  
[Guia Referência CSS](https://www.w3c.br/divulgacao/guiasreferencia/css2/)

[Propriedades CSS](https://www.todoespacoonline.com/w/2014/04/propriedades-css/)

[Box-model - Entendendo como funciona elementos no HTML](https://tableless.github.io/iniciantes/manual/css/box-model.html)

[Como utilizar a técnica CSS reset](https://www.devmedia.com.br/como-utilizar-a-tecnica-css-reset/26797)


[Devmedia - Utilizando media queries](https://www.devmedia.com.br/utilizando-css-media-queries/27085)

[Dimensionamento em CSS: px vs em vs rem ](https://chiamakaikeanyi.dev/sizing-in-css-px-vs-em-vs-rem/)

[Apostila HTML](https://www.alura.com.br/apostila-html-css-javascript/39CA-propriedades)

[Dimensionamento em CSS: px vs em vs rem](https://chiamakaikeanyi.dev/sizing-in-css-px-vs-em-vs-rem/)

[Efeito cascata, herança e especificidade no CSS](https://tableless.com.br/efeito-cascata-e-especificidade-do-css/)


[Como utilizar o google fonts](https://metring.com.br/como-utilizar-o-google-fonts/)

[Metodologia BEM para nomeação de classes e uso no CSS](https://medium.com/@fnandaleite/metodologia-bem-para-css-b0d3269b4853)


[Aplicando opacidade na cor](https://developer.mozilla.org/pt-BR/docs/Web/CSS/opacity)

[Propriedade object-fit para ajuste de imagens no CSS](https://cahfelix.com/entendendo-o-object-fit/)

[Centralizando conteúdos com `<div>s` no HTML](https://www.devmedia.com.br/como-centralizar-divs-em-html-e-css/37568)

