
# Medidas espaciales

En este ejemplo, vamos a estudiar un poco diferentes estrategias a la hora de definir tamaños para nuestro font y qué otras medidas puede afectar.

## Absoluto vs. relativo

A la hora de definir medidas, tenemos muchas variantes:

- píxeles (px), pulgadas (in), puntos (pt), centímetros (cm), milímetros (mm) y algunas otras medidas **absolutas**
- y las siguientes medidas **relativas**
  - em: toma como base el tamaño de la fuente del elemento padre
  - rem: toma como base el tamaño de la fuente del elemento raíz (el del `body`)
  - vh / vw: viewport height o viewport width, toma el 1% del tamaño del dispositivo (el tamaño variará dependiendo de que estés trabajando en un celular, una tablet, una ventana desktop o una de pantalla ancha)

Definir esto puede ser un poco confuso, en especial lo similar que parecen las definiciones de _em_ y _rem_, pero vamos a mostrarlo con un ejemplo.

## El ejemplo

El ejemplo se basa en una página que cuenta las bondades de una materia que enseña Interfaces de Usuario en una universidad:

![ejemplo](./images/ejemplo.png)

Como ven, podemos reconocer cuatro secciones:

- el header, que identifica el nombre de la materia y una breve descripción, dispuestos en un layout vertical, es decir cada uno ocupa una línea.
- el material, que tiene links a tres tecnologías. Aquí el layout es mixto: el contenedor tiene un layout horizontal, cada tecnología representa una columna, mientras que internamente el ícono y una breve descripción van con un layout vertical.
- el video de la semana, que cuyo contenedor utiliza un layout horizontal, y luego separamos el título del video de la semana y la descripción con un layout vertical
- y por último, los testimonios, que se forman con un contenedor cuyo layout es horizontal, y también es horizontal cada testimonio (la foto y la cita)

Gráficamente:

![layout ejemplo](./images/ejemplo_layout.png)

- en verde marcamos los layouts verticales, `flex-direction: column`
- en marrón los layouts horizontales, `flex-direction: row`

### Porcentajes

