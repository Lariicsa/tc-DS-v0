<p align="center">
  <a href="https://www.tucanton.com">
    <img alt="Tu Cantón" src="https://s3.amazonaws.com/tucanton/webapp/svg/tu-canton_logo.svg" width="100" />
  </a>
</p>
<h1 align="center">
  Guía de estilo y componentes
</h1>

_Entorno de desarrollo basado en React y diseño atómico para el diseño de Interfaz de Usuario_

## Índice

1. [Estructura](#Estructura)
1. [Colores](#Colores)
1. [Tipografías](#Tipografias)

## Colores

### SCSS

``
$white: rgba(255, 255, 255, 1);
$black: rgba(51, 51, 51, 1);
$primary: rgba(247, 148, 29, 1);
$primary-hover: rgba(247, 148, 29, 0.84);
$secondary: rgba(46, 196, 182, 1);
$grey: rgba(191, 185, 185, 1);
$grey-blue: rgba(189, 206, 219, 1);
$grey-bg: #f5f7f8;
$grey-bg-main: rgba(250, 250, 250, 1);
$mint: rgba(203, 243, 240, 1);
$yellow: rgba(255, 191, 105, 1);
$red: rgba(230, 59, 46, 1);
$accent: $secondary;
$text-color: $black;
$grey-dark: rgba(41, 57, 68, 1);
$grey-dark-2: rgba(35, 47, 59, 1);
$disabled-bg: rgba(250, 250, 250, 1);
$border-grey: rgba(162, 162, 162, 1);
$border-grey-dark: rgba(136, 144, 152, 1);

``

## Tipografías

**Rubik**

Se usa para 
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat...

``
@import url("https://fonts.googleapis.com/css?family=Rubik:400,500&display=swap");
``

**Karla**

``
@import url("https://fonts.googleapis.com/css?family=Karla:400,700&display=swap");
``

### SCSS
``
$font-text-main: "Karla", sans-serif;
$font-text-two: "Rubik", sans-serif;
$bold: 700;
$semibold: 500;
$regular: 400;
``

## Estructura base

    .
    ├── node_modules
    ├── src
      ├── SCSS
       ├── _mixins.scss
       ├── _vars.scss
       ├── global.scss
       ├── index.scss
       ├── normalize.scss
    ├── .gitignore
    ├── package.json
    └── README.md
