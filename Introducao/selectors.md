# Selectors

Conecta um elemento HTML com o CSS

## Tipos

* Global selector '*'
* Element/Type selector 'h1, h2, p, div'
* Id Selector '#box, #container'
* Class Selector '.red, .m-4'
* Attribute selector, Pseudo-class, Pseudo-element, e outros



``HTMl
<div id="container" class="m-40">
<h1>Titulo</h1>
<h2>Subtitulo<h2>
</div>







```CSS

margin: 0;
}

#container{
    width: 200px;
}

.m-40 {
    margin: 40px;
}

h1 , h2 {
    color:green;
    font-size: 60px;
    background: gray;
}