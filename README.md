# LM

Lenguaje de marcas HTML y CSS

## 1 ESTRUCTURA MINIMA DE UNA WEB.
```html
<!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>
</body>
</html>
```
## 2 EXPLICA LAS 3 FORMAS DE USAR CSS EN HTML.

### CSS Externo:
Se pone la direccion donde esta el archivo con el codigo css en la cabecera,dentro de <head></head>

EJEMPLO:
```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" type="text/css" href="EjemploEsteban.css" />
</head>
...
```

### CSS Interno:
De esta forma tambien se pone en la cabecera ,dentro de <head></head> pero tambien dentro de <style></style> y se va aplicando el codigo
desde ahí.

EJEMPLO:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo Css Interno Esteban</title>
    <style type="text/css">
        div {
            background:#FFFFFF;
        }
    </style>
</head>
...
```
### CSS Embebido:
En este caso no se pone en la cabecera si no que se aplica directamente al codigo html , usando el atributo style.

EJEMPLO:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo Css Embebido </title>   
</head>
<body>
  <p>Esteban<span style="color:#FF0000">Naranjo</span></p>
</body>
...
```
## 2 CREA UNA LISTA SIN ORDENAR CON 5 INGREDIENTES DE UNA RECETA DE COCINA.
