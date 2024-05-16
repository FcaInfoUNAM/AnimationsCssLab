# Animaciones con templates

Este repositorio tiene como objetivo revisar y adaptar a sitios web animaciones css creadar por terceros

Escribe en un archivo de texto llamado entregable.txt las respuestas a las preguntas del laboratrorio

## Paso1

Clona el repositorio en tu local
```cmd
git clone "{url}"
```

1. Visualiza las cards en el navegador
2. Haz click manteniendolo presionado en una card
3. Describe en el archivo entregable.txt que es lo que está sucediendo 

## Paso2

1. Revisa el documento css/animations.ss y ubica el apartado .card{} y modifica el código a como se muestra a continuación
```css
.card{
    -webkit-animation: slit-in-diagonal-2 450ms linear both;
    animation: slit-in-diagonal-2 450ms linear both;
}
```
2. Refresca la página y describe lo que pasa en el archivo entregable.txt
3. Modifica el código a como se muestra a continuación
```css
.card:hover{
    -webkit-animation: slit-in-diagonal-2 450ms linear both;
    animation: slit-in-diagonal-2 450ms linear both;
}
```
4. Refresca el sitio web y pasa el mouse por encima de los cards
5. Revisa el siguiente enlace [w3schools](https://www.w3schools.com/cssref/css_selectors.php)
6. Elige 3 selectores y pruebalos con el elemento card

## Paso 3

1. Revisa el siguiente enlace [https://animista.net/](https://animista.net/)
2. busca las animaciones de background y selecciona una
3. copia el código de los keyframes a animation css por ejemplo:
```css
/* BACKGROUND IMAGE*/
@-webkit-keyframes kenburns-top {
    0% {
    -webkit-transform: scale(1) translateY(0);
            transform: scale(1) translateY(0);
    -webkit-transform-origin: 50% 16%;
            transform-origin: 50% 16%;
    }
    100% {
    -webkit-transform: scale(1.25) translateY(-15px);
            transform: scale(1.25) translateY(-15px);
    -webkit-transform-origin: top;
            transform-origin: top;
}
}
@keyframes kenburns-top {
    0% {
    -webkit-transform: scale(1) translateY(0);
            transform: scale(1) translateY(0);
    -webkit-transform-origin: 50% 16%;
            transform-origin: 50% 16%;
    }
    100% {
    -webkit-transform: scale(1.25) translateY(-15px);
            transform: scale(1.25) translateY(-15px);
    -webkit-transform-origin: top;
            transform-origin: top;
    }
}
```
4. implementa el código a las imagenes del card con un selector, por ejemplo:
```css
.card-img-top:hover{
    -webkit-animation: kenburns-top 5s ease-out both;
    animation: kenburns-top 5s ease-out both;
}
```
4. Explica para qué funciona un keyframe en el archivo entregable.txt
5. Explica 3 propiedades de las animaciones que seleccionaste por ejemplo
```
transform permite modificar elementos pueden ser trasladados, rotados, escalados o sesgados de acuerdo a los valores establecidos
```
en el archivo entregable.txt

## Paso 4

1. Implementa una animación de texto en algún elemento del navbar
2. Implementa animaciones en el los botones del card al hacer hover y al hacer click

## Paso5
1. Guarda los cambios
2. Agrega los cambios a tu repositorio junto al archivo entregable.txt
``` git add entreganle.txt ```
``` git add animations.css ```
3. Haz una rama llamada entregable
``` git branch entregable ```
4. Cambiate a la rama recién creada
``` git checkout entregable ```
5. Realza un push sobre la rama
``` git commit -m "entregable" ```
``` git push origin entregable ```
6. solicita un pullrequest en github