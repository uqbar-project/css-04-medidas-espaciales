
# Medidas espaciales

En este ejemplo, vamos a estudiar un poco diferentes estrategias a la hora de definir tamaños para nuestro font y qué otras medidas puede afectar.

## Absoluto vs. relativo

A la hora de definir medidas, tenemos muchas variantes:

- píxeles (px), pulgadas (in), puntos (pt), centímetros (cm), milímetros (mm) y algunas otras medidas **absolutas**
- y las siguientes medidas **relativas**
  - em: toma como base el tamaño de la fuente del elemento padre
  - rem: toma como base el tamaño de la fuente del elemento raíz (el del `body`)
  - vh / vw: viewport height o viewport width, toma el 1% del tamaño del dispositivo (el tamaño variará dependiendo de que estés trabajando en un celular, una tablet, una ventana desktop o una de pantalla ancha)

Definir esto puede ser un poco confuso, en especial lo similar que parecen las definiciones de _em_ y _rem_, pero vamos a ponerlo con un ejemplo.

