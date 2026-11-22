## Proyecto Integrador (Información)
Nombre: Faisal Baroudi Tarfa
Nombre de usuario de GitHub: faisxl20
Correo electrónico: faisalbaroudi14@gmail.com

## Palabra del día 05/11/2026
Día

## Historial general de commits
Al reorganizar las carpetas, el historial de esta ruta muestra el commit que registra el traslado. Los commits anteriores siguen apareciendo en el historial general de `main`: https://github.com/faisxl20/Lenguaje_de_Marcas/commits/main

## UD3 · Estructura HTML
Al revisar mi `index.html`, he visto que:
1. La cabecera necesita una descripción, palabras clave y el nombre del autor; además, el título debe seguir el formato «Inicio | Nombre del proyecto».
2. El cuerpo necesita el comentario del menú NAV y secciones agrupadas en bloques `div` comentados. También debo completar la jerarquía de títulos con al menos dos `h2` y dos `h3`.
3. Faltan elementos de contenido solicitados: un `hr`, una cita `blockquote` con dos párrafos y su autoría, una ficha alineada en `pre`, y un pie con entidades HTML.

### Validación W3C

| Página | Resultado | Errores |
|---|---|---:|
| `index.html` | Validada sin errores | 0 |
| `leyendas.html` | Validada sin errores | 0 |
| `palmares.html` | Validada sin errores | 0 |
| `aficion.html` | Validada sin errores | 0 |

### Qué he hecho en esta unidad

He completado la estructura HTML de la portada y he creado las páginas de leyendas, palmarés y afición según el mapa del sitio. He añadido metadatos, jerarquía de títulos, bloques comentados, citas y fichas de datos. He validado las cuatro páginas con W3C y todas han obtenido cero errores.

## Mapa del sitio

| Fichero | title | Qué contiene |
|---|---|---|
| `index.html` | Inicio \| SEVILLA FC | Portada del proyecto. |
| `leyendas.html` | Leyendas \| SEVILLA FC | Todas las leyendas que aparecen en `index.html`, con sus datos tal como aparecen en `datos.xml`. |
| `palmares.html` | Palmarés \| SEVILLA FC | Los títulos del Sevilla FC. |
| `aficion.html` | Afición \| SEVILLA FC | La afición sevillista y Biris Norte. |
| `contacto.html` | Contacto \| SEVILLA FC | Página con formulario para que los aficionados envíen dudas o soliciten información. |



## Evidencia del commit de la palabra del día
El commit original se realizó en el repositorio `faisxl20/Proyecto` el 22 de octubre de 2026 a las 14:14:35 (hora peninsular española). Su mensaje es `Palabra del dia nueva añadida al README` y su hash es `75c2a608f0f25f5d851864f2489c627baa5696d3`. [Ver el commit original en GitHub](https://github.com/faisxl20/Proyecto/commit/75c2a608f0f25f5d851864f2489c627baa5696d3). Posteriormente, su historial se integró en este repositorio.

## Declaración de IA en commit
Al intentar subir los cambios desde la carpeta original, vi que estaba vinculada a otro repositorio, el motivo no se cual es y no podía publicarlos directamente en main. Pedí ayuda para integrar ambos historiales sin borrar ni sobrescribir el trabajo. La integración quedó registrada en un merge commit. Tambien he usado la IA para rescatar el primer commmit porque se hizo push en una rama ajena a la del repositorio y le he pedido que me ayude a rescatarlo y que me escriba la evidencia para que la profesora pueda entender que es lo que ha pasado y así no perder la puntuación de ese criterio.

## UD5 · Tablas y formularios

En la tabla de `palmares.html` voy a organizar por ámbito y competición los títulos del Sevilla FC, con el número y los años en que se ganaron.
El formulario de `contacto.html` servirá para que los visitantes envíen consultas sobre el Sevilla FC y sus competiciones.

### Prueba con GET y por qué uso POST

Al cambiar el formulario a `method="get"` y pulsar enviar, la URL que me salió en la barra del navegador fue:
`contacto.html?nombre=Faisal+Baroudi&email=faisal%40correo.com&telefono=612345678&clave_socio=1890&motivo_consulta=abonos&zona_estadio=gol_norte&notificaciones=partidos&mensaje=Deseo+informacion+sobre+los+abonos+de+esta+temporada.`

Uso `post` en vez de `get` porque con `post` los datos no se ven en la barra de direcciones ni se quedan guardados en el historial, lo que es mucho más seguro para proteger datos como el correo, el teléfono o la clave de abonado.

### Validación W3C

| Página | Resultado | Errores |
|---|---|---:|
| `palmares.html` | Validada sin errores | 0 |
| `contacto.html` | Validada sin errores | 0 |

Al pasar los dos archivos por el validador del W3C no me ha dado ningún error, ya que las etiquetas de la tabla, los fieldset y los controles estaban bien estructurados y cerrados.

### Qué he hecho en esta unidad

En esta unidad he añadido a la página de palmarés una tabla con los títulos que ha ganado el Sevilla FC, organizándola con cabecera, cuerpo y pie, y agrupando las competiciones con `rowspan` y `colspan`. Además, he creado la página de contacto con un formulario completo para los aficionados, con sus dos bloques, opciones personalizadas sobre el club y campos obligatorios. Por último, he enlazado la nueva página en la portada y he comprobado que todo valida sin fallos en el W3C.


## Tarea 6-7

En esta práctica he seguido mejorando mi página web sobre el Sevilla FC aplicando los conceptos que hemos estudiado en clase durante los temas 6 y 7 de Lenguaje de Marcas.

### 1. Estructura semántica en HTML5 (Reto 1)
Antes tenía la página organizada usando muchos bloques `<div>` genéricos. Siguiendo lo que hemos dado en el Tema 6, he reestructurado tanto `index.html` como `palmares.html` y `contacto.html` para usar etiquetas semánticas con significado real:
* He colocado un `<header>` arriba con el escudo, el título principal del club y una pequeña introducción.
* He añadido la barra de menú con `<nav>` enlazando a todas las páginas de mi sitio (`index.html`, `palmares.html`, `leyendas.html`, `aficion.html` y `contacto.html`) para que el usuario pueda navegar cómodamente.
* Todo el contenido central lo he metido dentro de un único `<main>`, dividiéndolo en secciones con `<section>` y artículos con `<article>` (por ejemplo, para la historia de las leyendas y los títulos de Europa League).
* A un lado he puesto un `<aside>` con datos rápidos del estadio y del club en texto preformateado (`<pre>`), además de enlaces de interés.
* En el pie de página (`<footer>`) he añadido mi firma con el identificador que pedía la profesora: `<p id="firma-faisxl20">© 2026 Faisal Baroudi Tarfa (faisxl20)</p>`, y he actualizado el `<meta name="author" content="faisxl20">` en la cabecera de los archivos.

### 2. Formulario y elementos de medición (Reto 2)
En la página `contacto.html` he ampliado el formulario de atención al sevillista para practicar los nuevos controles de HTML5:
* He añadido 7 tipos de `input` nuevos que vimos en el tema: `email`, `tel`, `date` (para elegir fecha de nacimiento), `url` (para la web de la peña), `number` (para pedir entre 1 y 6 entradas), `range` (una barra deslizante para indicar del 1 al 10 con qué frecuencia vas al estadio) y `color` (para seleccionar el color de la bufanda sevillista).
* Para las validaciones he usado `required`, `placeholder`, `min`, `max`, `step` y `autofocus` en el primer campo. Además, para el carné de socio he puesto una expresión regular con `pattern="SFC-[0-9]{5}"` y un `title` que te explica el formato si te equivocas (por ejemplo, `SFC-12345`).
* Antes del formulario he incluido dos elementos de medición del Tema 6:
  * Un `<progress>` para ver cómo va la campaña de renovación de abonos (al 85%).
  * Un `<meter>` para indicar de forma gráfica el aforo medio ocupado en el Ramón Sánchez-Pizjuán (39.500 espectadores sobre un máximo de 43.883).

### 3. Vídeo, figuras y preguntas frecuentes (Reto 3)
En la portada `index.html` he añadido una sección multimedia para hacer la web más entretenida:
* He creado la carpeta `media/` donde he guardado el vídeo del himno en el estadio cantado por la afición en dos formatos distintos (`.mp4` y `.webm`), con su carátula (`poster="media/poster_himno.jpg"`) y la barra de controles (`controls`), pesando menos de 10 MB. También he añadido el audio en `.mp3` y `.ogg`.
* Además, como la profesora permitía incluir un vídeo de YouTube, he incrustado con un `<iframe>` el vídeo oficial del himno del centenario en el Sánchez-Pizjuán.
* He puesto dos fotos con `<figure>` y su pie explicativo en `<figcaption>` (una del estadio y otra de las 7 copas de la Europa League).
* Para las dudas he creado una sección de preguntas frecuentes con tres desplegables usando `<details>` y `<summary>`. Una de las preguntas viene abierta por defecto con `open`, y en otra he explicado cómo se hace la tabla de títulos escribiendo las etiquetas con las entidades `&lt;table&gt;` y `&lt;th&gt;` para que el navegador no las confunda con código.

### 4. Hoja de estilos externa (Tema 7)
He creado la carpeta `css/` con el archivo `estilos.css` y lo he vinculado en el `<head>` de todas las páginas con la etiqueta `<link rel="stylesheet" href="css/estilos.css">`.
Para no meter cosas que no hayamos dado en clase, me he limitado estrictamente a las propiedades y selectores del Tema 7:
* He usado el selector universal `*` para quitar los márgenes y rellenos por defecto que meten los navegadores (`margin: 0; padding: 0`).
* He definido los colores oficiales del Sevilla FC usando valores hexadecimales: blanco (`#ffffff`), rojo sevillista (`#d4001f` y `#c8102e`) y un gris oscuro (`#222222`) para que los textos sobre fondo claro se lean cómodamente.
* He organizado el modelo de caja usando `margin`, `padding` y `border: solid ...` en la cabecera, los títulos, la tabla de palmarés y los bloques del formulario.
* Para los anchos he usado porcentajes (`width: 90%`, `width: 95%`) y píxeles (`px`), además de tamaños de letra en `rem` y `px`.
* En los selectores he practicado selectores de etiqueta (`table`, `th`, `td`), selectores descendientes (`nav ul`, `nav a`, `table th`), selectores de ID (`#firma-faisxl20`) y selectores de atributos para darle estilo propio a los botones de enviar y borrar del formulario (`input[type="submit"]` e `input[type="reset"]`).

### 5. Cómo queda la carpeta de mi proyecto
```text
Proyecto-Integrador-LM-2026/
└── Proyecto/
    ├── index.html (portada con la estructura HTML5, multimedia y enlaces)
    ├── palmares.html (página con la tabla de títulos y diseño CSS)
    ├── contacto.html (formulario con nuevos inputs y barras progress/meter)
    ├── leyendas.html (lista de jugadores históricos con estilos aplicados)
    ├── aficion.html (historia de la afición sevillista y peñas con estilos)
    ├── datos.xml (archivo de datos en XML del club)
    ├── Readme.md (documentación del proyecto y notas de cada tema)
    ├── css/
    │   └── estilos.css (hoja de estilos CSS externa del Tema 7)
    ├── media/
    │   ├── copas_europa_league.jpg (foto para el figure de trofeos)
    │   ├── estadio_sanchez_pizjuan.jpg (foto para el figure del estadio)
    │   ├── himno_sevilla_estadio.mp4 (vídeo local en formato MP4)
    │   ├── himno_sevilla_estadio.webm (vídeo local en formato WebM)
    │   ├── himno_sevilla_estadio.mp3 (audio en MP3)
    │   ├── himno_sevilla_estadio.ogg (audio en OGG)
    │   └── poster_himno.jpg (carátula del vídeo)
    ├── img/
    │   └── escudo_sevilla_fc.png (escudo del club)
    └── capturas/
        └── captura_portada_navegador.png (captura de la portada en el navegador con CSS)
```

### 6. Historial de commits realizados
He ido trabajando paso a paso, comprobando los cambios en el navegador antes de cada commit para que el historial refleje el avance real:
1. `chore: inicio tarea 6-7` (commit inicial que pedía la profesora al empezar).
2. `feat: estructura semántica html5 en index` (primera versión semántica de la portada).
3. `feat: estructura semántica html5 en palmares` (semántica en la página del palmarés).
4. `feat: formulario con controles html5` (formulario de contacto con inputs y elementos de medición).
5. `feat: video, figuras y preguntas frecuentes` (sección multimedia, fotos con pie y dudas en portada).
6. `style: estructura base, colores y tipografia en css` (creación de estilos.css y enlace en todas las páginas).
7. `style: navegacion, tabla de titulos y formulario` (diseño de la barra del menú, tabla y campos).
8. `style: multimedia, figuras, preguntas frecuentes y barra lateral` (diseño de vídeos, imágenes y desplegables).
9. `docs: documentacion y entrega final tarea 6-7` (documentación en el README y carpeta de capturas).