# Shorthand

* junção de propreidades
* resumido
* legivel

````css

{
        /* background properties */
        background-color: #000;
        background-image: url(image/bg.gif);
        background-position: no-repeat;
        background-position: left top;


        /* background shorthand*/   
        backgroind: #000 url(images/bg.gif) no-reapet left top;

        /* font preperties */
        font-style: italic;
        font-weight: bold;
        font-size: .8em;
        line-height: 1.2;
        font-family: Arial, sans-serif;    


        /* font shorthand */
        font: italic bold .8em/1.2 Arial, sans-serif;
}
´´´´

## Detalhes

* nao ira considerar propriedades anteriores
* valores nao especificados irao assumir o valor padrao
* geralmente, a ordem descrita nao importa, mas, se houver muitas propriedades
com valores semelhantes, poderemos encontrar problemas 