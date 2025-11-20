📘 Dashboard Responsive – Práctica de Layout Adaptativo

Este proyecto consiste en crear un layout adaptativo (responsive) usando Media Queries y Flexbox, siguiendo el enfoque mobile-first.
El objetivo principal es transformar un diseño vertical (una columna) en móvil, a un diseño de dos columnas en pantallas más grandes (desktop/tablet).

✔ Requerimientos cumplidos
1. Diseño Mobile-First

El proyecto inicia con un layout en una sola columna:

Sidebar arriba

Contenido abajo

Tarjetas apiladas verticalmente

2. Transformación del layout con Media Query

En el archivo styles.css, se utiliza:

@media (min-width: 768px) {
    ...
}


A partir de 768px, se transforma el diseño a modo escritorio.

3. Flexbox aplicado al layout principal

En escritorio, el contenedor .main-layout se convierte en un contenedor flex:

Sidebar en la izquierda

Contenido principal a la derecha

Con separación entre columnas

4. Sidebar con ancho definido

El sidebar usa:

flex: 0 0 250px;


Lo que le da un ancho fijo.

5. Contenido flexible

El área de contenido usa:

flex: 1;


Para ocupar automáticamente el espacio restante.

6. Tarjetas de noticias adaptadas

En móvil, las tarjetas están en columna.
En escritorio, el media query las convierte en:

Dos tarjetas por fila

Con flex-wrap para que se ajusten al espacio

📁 Archivos del proyecto
index.html
styles.css
README.md

📌 Descripción breve del funcionamiento

El proyecto usa CSS externo.

El layout es de una columna en móvil.

A partir de 768px, se activa un diseño de dos columnas usando flexbox.

Las tarjetas también cambian de estructura para adaptarse al tamaño de pantalla.
