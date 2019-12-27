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

1. [Breakpoints](#Breakpoints)
1. [Colores](#Colores)
1. [Tipografías](#Tipografías)
1. [íconos](#íconos)
1. [Estructura](#Estructura-base)

## Colores

### variables en SCSS 

- $white
- $black
- $primary
- $primary-hover
- $secondary
- $grey
- $grey-blue
- $grey-bg
- $grey-bg-main
- $mint
- $yellow
- $red
- $accent
- $text-color
- $grey-dark
- $grey-dark-2
- $disabled-bg
- $border-grey
- $border-grey-dark


## Tipografías

**[Rubik](https://fonts.google.com/specimen/Rubik)**

Se usa para 
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat...

``
@import url("https://fonts.googleapis.com/css?family=Rubik:400,500&display=swap");
``

**[Karla](https://fonts.google.com/specimen/Karla)**

Se usa para 
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat...

``
@import url("https://fonts.googleapis.com/css?family=Karla:400,700&display=swap");
``

### variables en SCSS 

- $font-text-main
- $font-text-two
- $bold
- $semibold
- $regular

## Íconos

### variables en SCSS 

Para la íconografía manejamos SVG en base64 en la hoja de [Mixins]( #Mixins.md )

- logo-color, logo a todo color

En la iconografía que tiene variables se manejan 2 variables: nombre del ícono y nombre del color

ejemplo: `` @include icon('heart', $red) ``

- icon($name, $color)
  - 'arrow'
  - 'calendar'
  - 'heart'
  - 'profile'
  - 'settings'
  - 'user'


## Breakpoints

Actualmente se manejan 3 tamaños en pantalla: 

- Default _Pantallas mayores a 768px_
- Tablet _Pantallas menores a 768px y mayores a 376_
- Mobile _Pantallas menores a 376_ 

### variables en SCSS 

- $tablet
- $mobile

En caso de requerir un punto específico se usa el mixin:

- until($device)

Inicadndo en la variable *$device* el punto máximo de pantalla

ejemplo: `` @include until('1024px') ``


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
