# project-zero

Ejercicio integrador de los conceptos vistos sobre HTML5.

## Parte 1

## Tiempo para resolverlo (Parte 1)

1 semana.

## Fecha de entrega (Parte 1)

21/23 de Marzo, dependiendo en qué grupo estés.

### Consigna

1. Dividirse en grupos de 2 estudiantes. 
2. Cada grupo tendrá que maquetar un artículo de una noticia (como si se tratase de la página de un diario online), creando su contenido (título, párrafo, imágenes, etc) en base a 3 palabras *aleatorias* que les serán asignadas. 
3. Investigar en [MDN](https://developer.mozilla.org/en-US/) sobre las etiquetas que no conozcan.
4. El documento **debe** que incluir las etiquetas que figuran en la [estructura](#estructura-del-sitio) que se encuentra debajo.
5. Se recomienda inspirarse y sacar ideas de sitios de noticias y artículos reales, por ejemplo [este](https://www.lanacion.com.ar/buenos-aires/los-portenos-eligieron-luccianos-como-mejor-heladeria-nid2229133).
6. Para realizar este ejercicio, tendrán que [forkear](https://help.github.com/en/articles/fork-a-repo) este repositorio y en *su nueva copia*, agregar un archivo `index.html` que contenga la solución.

### Estructura del sitio

```
header
    p [1]
    nav
        ul [2]
main               
    article
        section
            h1 [3]
        figure
                img [4]
                figcaption
        section
            p [5]
    aside
        img [6]

footer
    p [7]
    a [8]
    a [9]
```

[1]: Título del diario.  
[2]: Lista de tematicas/secciones. Acá marcamos en negrita (y en otro color) la que corresponda, es decir, la actual donde estamos ahora.  
[3]: Título de la noticia.  
[4]: Imagen relacionada a la noticia. Debe tener los atributos `src` y `alt`!  
[5]: Texto con el contenido de la noticia. Debe tener links (absolutos o relativos) en alguna parte del texto para leer más sobre algún tema.  
[6]: Imagen de publicidad/spam, preferentemente relacionada al contenido de la noticia.  
[7]: Texto de Copyright.  
[8]: Link absoluto hacia algún sitio externo.  
[9]: Link que nos lleve hacia el header del diario (usar `id=header` para identificarlo).  


Camilo

