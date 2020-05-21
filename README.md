## React coding challenge

Se creara un componente simple de React: Un selector de avatar. La idea es que quede como el siguiente gif:

![Pick an avatar](./avatar_picker.gif "Seleccioname!")

El usuario podrá hacer click sobre el avatar y se abrira un pop up que permitira cambiar dicho avatar. Luego del click para seleccionar el nuevo avatar se tendrá que simular un request http fake, el cual se simulara con un spinner de carga (como se muestra en el archivo anterior. Luego de simular la carga se debe cerrar el pop up mostrando el nuevo avatar seleccionado en la pantalla inicial.

### Diseño y comportamiento:

* El avatar inicial a mostrar es el primero de la lista.
* El avatar actual debe aparecer con borde de 1px.
* Los grupos de avatar se deben mostrar en grupo de 4, (como muestra en el gift).
* El pop up se abre con animación.
* El avatar que se realiza hover debe aparecer con un borde de 3px en azul.
* El spinner de loading debe aparecer como se muestra en el gif.
* Realizar click por fuera del pop up lo debe cerrar.
* La simulación del request en el spinner debe ser de un segundo.
* El pop up se cierra luego que se ejecuto el fake request al elegir el nueva avatar.

### Colores y medidas:

* Imagen del Avatar
  * height: 60px, width: 60px, perfect circles
  * border for initial image: hover, focus 1px, color: rgb(155, 160, 163)
  * Lista de avatar:
    * border en hover: 3px border, color rgb(155, 160, 163);
    * overlay en hover: color rgb(122, 161, 178), opacity: 20%
    * border spinner, currently active avatar: color: rgb(122, 161, 178)
    * margin entre dos avatars: 14px
* Pop up
  * width: 280px
  * height: variable
  * rounded corners of 2px radius
  * background: rgb(44, 48, 51)
  * drop shadow: color: rgb(102, 102, 102), size 2px, blur 10px
  * padding: 14px
  * triangle: equilateral, 8px each side
  * Título: "Selecciona el avatar"
  * font: 'Source Sans Pro' (use the google font)
  * color: rgb(249, 249, 249)
  * size: 16px
  * margin top and bottom: 14px

### Instrucciones:

* La siguiente lista es la que se pasara como property al nuevo componente. El id es único y se asegura que va a venir la imagen en el directorio root.


```
[
  { "src": "avatar1.png", "label": "Avatar 1", "id": 1 },
  { "src": "avatar2.png", "label": "Avatar 2", "id": 2 },
  { "src": "avatar3.png", "label": "Avatar 3", "id": 3 },
  { "src": "avatar4.png", "label": "Avatar 4", "id": 4 },
  { "src": "avatar5.png", "label": "Avatar 5", "id": 5 },
  { "src": "avatar6.png", "label": "Avatar 6", "id": 6 }
]
```

* Usted debe determinar como descomponer en componentes el componente principal.
* Piense que este componenete sera parte de una aplicación mucho mayor, y que se podrá reutilizar.
* Se puede utilizar cualquier librería de JS de terceros.
* No se puede usar librerías de css de terceros.
* Solo se pueden utilizar las imagenes dadas, sin que sean modificadas para que se adapten.
* Se deben utilizar los tags HTML semanticos(por ejemplo: la lista de avatar tienen que ser `<ul>` y los hijos `<li>`)
