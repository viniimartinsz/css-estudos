# A CASCATA (cascading)

A escolha do browser de qual regra aplicar, caso haja muitas regras para o mesmo elemento

* Seu estilo é lido de cima para baixo

È levado em consideração 3 fatores

1. Origem do estilo
2. Especificidade
3. Importancia


### Origem do estilo

Inline > tag style > tag link


### Especificidade

È um calculo matematico, onde, cada tipo de seletor e origem do estilo, possuem valores a serem considerados.

0. Iniversal selector, combinators e negation pseudo-class (:not())
1. Element typep selector e pseudo-elements (::before, ::after)
10. Classes e attribute selectors ({type="radio"}
100. ID selector
1000. Incline

### A regra !important

* cuidado, evite o uso
* não é considerado uma boa pratica
* quebra o fluxo natural da cascata

HTML
<h1 class="title" id="my-title" style="color:orange;">Titulo</h1>
<p>paragrafo</p>             <!--  1 ordem --!

```css

#my-title {
    color:gray;     /*  2 ordem */
}
.title{
    color: red;    /* 3 ordem */
}
h1 {
    color:red;
}
h1 {
    color:blue;                     /* VAI FICAR AZUL = (CASCATA)
    
                                        DE CIMA PARA BAIXO  */
}


h1.title#my-title {
    color:blue         /* MAIOR FORÇA */
}