# postcard-form

Partiendo del html que se facilita construir el siguiente formulario:

![postal](https://imgur.com/BtKM9i1.png)

Add the above code into the body of your HTML.

## Organiza los recursos que necesitas:
- El fondo de postal: guardado en el directorio de trabajo del HTML.
- Obtener la fuente de escritura de máquina de escribir: The "Secret Typewriter" de la página [fontsquirrel](www.fontsquirrel.com )
- Obtener la fuente de escritura a mano: The "Journal"  de la página [fontsquirrel](www.fontsquirrel.com )

_Para procesar las fuentes seguir los pasos siguientes: _

1. Utilizar el generador de fuentes de fontsquirrel: __fontsquirrel Webfont Generator__.
2. Utilizando el formulario subir ambos ficheros de las fuentes y generar un _webfont kit_. Descargar al ordenador
3. Hacer unzip del fichero.
4. Dentro del contenido copiar los cuatro ficheros: dos .woff y dos .woff2 a una carpeta fonts dentro del directorio de trabajo.

## La sección CSS

1.- Preparar las reglas @font-face rules, el elemento reset `<body>` y el `<form>` (w: 740px h:498px y bck: imagen + color white):
2. Posicionar los elementos del título y del form
3. Trabajar los elementos del form:
    - Fuente título: 1 em typewriter, sans-serif
    - Labels .8 em typewriter, sans-serif
    - Eliminar bordes y fondo de los campos de texto. Redefinir padding y margen.
    - Resaltar los campos con foco con un background light grey, transparent (utilizar la propiedad outlinge para eliminar el borde).
    - El elemento `<textarea>` debe renderizarse como elemento de bloque al que se debe anular las propiedad resize. 
    - Utilizar pseudo-elementos para añadir los ">>>" al botón. 
    - El botón rota -1.5deg.

