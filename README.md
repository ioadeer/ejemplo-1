# Aurora Studio (versión resuelta)

Este ejemplo muestra cómo conectar un servicio como Formspree con Javascript.
Partiendo de ejemplo_1/resuelto

# Instrucciones

Ingresar a Formspree, crear un usuario.
En el dashboard 
- Add New
- New Form

## En conctact.html

Agregar el id="contactForm" al elemento <form></form>


Agregar

```{html}
 <!-- <p></p> vacío para guardar status de respuesta -->
 <p id="form-status" aria-live="polite"></p>
```
antes del botón.


Agregar el id="submitButton" al elemento ```<button></button>``` del formulario

Crear una carpeta, llamarla js y crear un archivo con el nombre form.js dentro.

Agregar

```{html}
    <!-- Link a un script -->
    <script src="js/form.js" defer></script>
```

al final de 

```{html}
<main></main>.
```

## En js/form.js

Agregar

```{javascript}
const ENDPOINT = 'https://formspree.io/f/mi-codigo'
```

## En css/styles.css

Agregar, por ejemplo

```{css}
    --ok:#146c2e;
    --danger: #FF0000;
```

en la parte de mi archivo donde delcaro las variables con el fin de colorear los errores.
