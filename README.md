# project-zero

Ejercicio integrador de los conceptos vistos sobre HTML5.

## Parte 1

### Fecha de entrega (Parte 1)

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

---

## Parte 2

### Fecha de entrega (Parte 2)

28/30 de Marzo, dependiendo en qué grupo estés.

### Consigna

Para esta 2da parte, vamos a comenzar a aplicar estilos a nuestro sitio y hacer algunas modificaciones a nuestro documento. Al final se incluye una imagen de referencia para visualizar mejor las modificaciones.

#### Importante

- Esta 2da parte **NO** incluye modificaciones del CSS correspondiente al *layout* del contenido (los elementos en bloque seguirán quedando uno debajo del otro), eso quedará para la 3ra. parte del proyecto.
- El proyecto debe resolverse con el mismo grupo con el que hiciste la 1er parte del mismo.
- Utilizar **Git y GitHub** para colaborar y trabajar en conjunto.
- Ambos miembros del equipo deben presentar **el mismo proyecto**, no 2 versiones individuales.
- Se va a evaluar la **reutilización de estilos en CSS**. También que, preferentemente se utilicen selectores de clase sobre cualquier otro.

#### Estilos CSS

1. *Aplanar* lista de temáticas/secciones, es decir, que la lista se vea horizontal, con los ítems uno al lado del otro.
2. Sacarle los bullets/viñetas a la lista de temáticas/secciones.
3. Definir un tamaño base para la fuente de nuestro documento en `18px`.
4. Definir un tamaño relativo para los `h1` que sea 2.25 veces más grande que el tamaño base.
5. Definir un tamaño relativo para los `h2` que sea 1.75 veces más grande que el tamaño base.
6. Definir un tamaño relativo para los `h3` que sea 1.4 veces más grande que el tamaño base.
7. Definir el color `#fafafa` como color de fondo de nuestro sitio.
8. Definir el color `#24292e` como color para el texto de nuestro sitio (`h1`, `h2`, `h3` y `p`).

#### Cambios en el HTML

La estructura de nuestro sitio va a modificarse ligeramente y quedar de esta forma

```
header
    p
    nav
        ul
main               
    article
        section
            h1
        figure
            img
            figcaption
        section
            p [10]
            p
            p
            figure
                img
                figcaption
            p [16]
    section [11]
            h2
        article
            h3
            figure
                img
                figcaption
        article
            h3
            figure
                img
                figcaption
    aside
        h3 [12]
        img

hr [15]
footer
    a [13]
    a [14]
    p
```

1. Agregar una nueva section [11] que contiene lo siguiente: 2 `articles`, correspondientes a 2 noticias recomendadas (no necesariamente relacionadas a la que estamos leyendo), con sus correspondientes títulos (`h3`) e imágenes descriptivas.
2. Agregarle un `h3` al `aside` que contiene la publicidad, con el texto `PUBLICIDAD` [12].
3. La noticia debe contener **al menos 3 párrafos** [10].
4. Agregar un `p` con un margen inferior de `30px`antes del primer párrafo de la noticia, en color `#808080` y tamaño `0.75` (respecto del tamaño base), que contenga el texto `<FECHA> - <HORA>`, ejemplo `23 de Marzo de 2019 - 12:36`.
5. Agregar una 2da imagen (con su correspondiente caption) relacionada a la noticia.
6. Agregar un `p`[16] al final del texto de la noticia, con un margen superior de `25px`, que contenga el texto "Por:" seguido de links absolutos a los perfiles de GitHub de lxs autores del proyecto (Por: [repo-user-1](#) - [repo-user-2](#)).
7. Agregar un `hr` [15] antes del `footer`, con un margen superior de `45px`y los siguientes estilos: `border: 0.5px solid #808080;`, ancho del 80% y opacidad `0.3`. 
8. Modificar el `footer` para que quede similar al de la imagen de referencia (ver abajo): un `p` con el texto Código fuente: [repo-1](#) | [repo-2](#), que linkee a los repositorios del sitio de cada autor del proyecto, el link de Volver al inicio debajo (ver siguiente ítem) y el texto de copyright centrado, entre ambos links.
9. El link restante del `footer` [14] debe continuar siendo un link con el texto "Volver al inicio", que nos lleve hacia el `header`del sitio.

#### Imagen de referencia

![](https://i.imgur.com/f5OIzcq.jpg)

---

## Parte 3

### Fecha de entrega (Parte 3)

11/13 de Abril, dependiendo en qué grupo estés.

#### Estilos CSS

1. Definir alguna tipografía distinta a la default para los `p`. Esta fuente debe ser [safe web](http://web.mit.edu/jmorzins/www/fonts.html) para asegurarnos compatibilidad independientemente del sistema operativo del usuario.
2. Elegir alguna fuente de [Google Fonts](http://fonts.google.com) para los `h1` y usarla con el `font-weight` correspondiente a `bold`.
3. Elegir otra fuente de [Google Fonts](http://fonts.google.com) para los `h2` y `h3`. Usarla con el `font-weight` correspondiente a `bold` (`h1`, `h2/h3` y `p`deben tener tipografías distintas).
4. Transformar los `h3` para que siempre se vean en mayúsculas.
5. Agregarle los estilos correspondientes a todas las imágenes del sitio para que sean *responsive*. **Pista:** alcanza con modificar ancho y alto de las mismas.
6. Modificar el estilo de los links (anchors) de nuestra página, para que no tengan subrayado y su color sea `#0074c4`.
7. Modificar el estilo de los links (anchors) de nuestra página, para que tengan el color `##0098ff`y subrayado al hacer *hover* sobre los mismos.
8. Flotar las secciones de publicidad y noticias recomendadas a la derecha para que se vean como en la imagen de referencia.
9. Dejar un margen de `24px`entre las secciones de publicidad y noticias recomendadas y el `article` correspondiente a la noticia.
