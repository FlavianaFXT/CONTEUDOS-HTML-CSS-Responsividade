# CONTEUDOS-HTML-CSS-Responsividade
Resumo de conteudo proveniente de cursos realizados na área de Front End nas seguintes comunidades:

Reprograma


## INDICE

### HTML
1. [Estruturas básicas](#topico3)
2. [HTML Semântico](#topico3)
3. [Class e ID](#topico3)

   
### CSS
1. [Link Style sheet](#topico4)
2. [USo de seletores](#topico4)
3. [Propriedades e valores](#topico4)

### Responsividade
1. [Mobile First](#topico4)
2. [Media Query](#topico4)
3. [Breakpoint](#topico4)
* [Entendendo sobre Responsividade](#Responsividade)
* [Tipos de imagem](#tiposdeimagem)
* [Unidade de medida](#unidadesdemedida)
* [Media Querie](#mediaquery)

### HTML

#### Estrutura básica
* [Principais Tags](#subtopico1)
* [HTML Semântico](#Subtopico2)

Com estes dois conceitos bem fixados, você vai longe!

##### Principais tags

- Tags estruturais: **html, meta,body, main, style, link,  title**
- Cabeçalho : **header, nav**
- Titulos: **h1 a h6**
- Parágrafo : **p**
- Link : **a e seus atributos**
- Listas: **ol, ul e li**
- Imagem: **img**
- Formulários: **form, input, label, textarea, fieldset**
- Formulários: **p** **table, th, td, tr**
- Rodapé:  **footer**
- Outras: **div, section, br**
  

##### HTML Semântico
O HTML semântico foi criado com o intuito de aproximar a linguaguem do HTMl da linguagem comum, usual, facilitando a leitura da desenvolvedora, auxiliando na indexação da página pelo Google, além de melhorar a acessibilidade no uso de leitores de tela.

* nav
* main
* article
* header
* aside
* footer
* section

#### Class e ID

As tags podem ser nomeadas de acordo com o conteúdo da página que está sendo criada para facilitar a estilização e possibilitar que uma tags com o mesmo nome possam ter estilos diferentes no css.

Para chamá-los, o padrão é:

```
  <p class="paragrafo"> Ola </p>

```
```
  <header>
  <p> Ola </p>
  </header>

```

Com o método **BEM** os nomes das classes e seletores seguem um padrão diferencia aquilo que é um conteúdo de bloco **B**, elemento **E** e modificadores **M**.
Utilizar o BEM é benefíco, rsss! 😅

### CSS

#### Link stylesheet

Para que a página tenha a sua estilização incluir a **tag style* dentro da *tag head*.
Há outras formas de chamar a taga style, mas a forma mais indicada é seguida abaixo:

```
    <link rel="stylesheet" href="style.css">

```

Criando um arquivo com extensão **css**, este arquivo é linkado conforme exemplo acima. Confira se o caminho incluido no **atributo href** está correto.

#### Uso de seletores

Para que seu conteúdo seja estilizado, é preciso chamar os seletores.
Os seletores são as tags e os nomes das class e id que você criou no html.

Exemplos:

```
    h1 {
      propriedade: valor;
    }

    h1, p{
      propriedade: valor;
    }

    .titulo {
      propriedade: valor;
    }

    .titulo__secundario {
      propriedade: valor;
    }

    footer > .titulo__rodape{
      propriedade: valor;
    }

    #article {
      propriedade: valor;
    }

```
#### Propriedades e valores

O CSS tem propriedades específicas para a estilização de cada tag/elemento. Nestas propriedades se encontram diversos valores utilizados de maneira generalizada e outros específicos.

```
   h1 {
      font-style: italic;
    }

   img {
    width: 100%;
   }

   p {
    font-size: 1.5em;
   }

```

Lembrando que o HTML já tem padrões para as tags e, quando utilizamos a estilização, mudamos estes padrões.
CSS é estudo, erro, estudo, acerto e erro de novo.

![css](https://media.giphy.com/media/YFkpsHWCsNUUo/giphy.gif)

### Responsividade

O layout responsivo traz fluidez para as nossas páginas, possibilitando  o uso do mesmo layout  de acordo com o tamanho da tela.
: **celular, table, desktop, laptop e televisão*.

As alterações no CSS acontecem com  o uso da técnica **media query**. Nesta técnica incluimos os break points - os pontos de quebra dos tamanhos das telas. 

#### Mobile first

A responsividade tem o conceito  **mobile first**, que orienta a estilização da página primeiro para o formato mobile(celular). Isso facilita o acesso de diversos usuários que têm o celular como principal meio de acesso à internet.

#### Media query

Media Query é a técnica que indica ao CSS que a partir da inserção da informação **@media (largura em px)** o layout terá outro comportamento.
É importante deixar o conteúdo que seja importante e necessário para a compreensão do usuário.

#### Breakpoints

O break point é o ponto em que a "tela quebra". Ele indica que a partir de determinada largura haverá uma mudança no layout da página telas mobile, tablet, laptop ou desktop.
Há um padrão dos break point que são mais utilizados, devido os diversos tamanhos de telas.


- Box Model 
- Formularios 


* BEM
- [bem](https://desenvolvimentoparaweb.com/css/bem/)

* text-align
- [text-align](https://www.w3schools.com/cssref/pr_text_text-align.php)

  
##### extra de CSS:

- [Justfy-content](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content)
- [flex-direction](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-direction)
- [grid](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column)
- [position](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning)
- [Display](https://github.com/reprograma/html-css-basico)
- [Display](https://developer.mozilla.org/en-US/docs/Web/CSS/display)


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

- [Principais Tags HTML](https://www.codigofonte.com.br/artigos/principais-tags-de-html)
- [O que é HTML Semântico](https://ayltoninacio.com.br/blog/o-que-e-html-semantico)
- [Método BEM](https://en.bem.info/methodology/html/)
- [Propriedades CSS](https://www.alura.com.br/apostila-html-css-javascript/39CA-propriedades)
- [Breakpoints de maneira coerra](https://desenvolvimentoparaweb.com/css/css-breakpoints-maneira-correta/)

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

