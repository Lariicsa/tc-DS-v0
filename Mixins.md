
# SCSS Mixins

Actualmente se manejan imágenes SVG para iconografía en formato base 64, y la manipulación se hace a través de una clase de SCSS establecida en el archivo *_mixins.scss*

## Como llamar en SCSS

- Logo a color

```css 
@include logo-color;
```

- Ícono de error

```css 
@include icon-danger;
```

## Set de íconos modificables

La variable *$name* es de acuerdo al ícono que se seleccione

La variable *$color* es el color que se desee modificar en la imagen

```css 
@include icon($name, $color);
```

- Ícono de calendario

```css 
@include icon('calendar', $primary);
```

- Ícono de corazón

```css 
@include icon('heart', $primary);
```

- Ícono de ávatar de perfil con relleno

```css 
@include icon('profile', $primary);
```

- Ícono de ajustes

```css 
@include icon('settings', $primary);
```

- Ícono de ávatar de perfil sin relleno

```css 
@include icon('user', $primary);
```

## Set de breakpoints

- Tamaño Tablet

```css 
@include tablet;
```

- Tamaño teléfono

```css 
@include mobile;
```

- Tamaño personalizado hasta cierta medida

```css 
@include until('Npx');
```