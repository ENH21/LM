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
Se pone la direccion donde esta el archivo con el codigo css en la cabecera , dentro de ```<head></head>```

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
De esta forma tambien se pone en la cabecera ,dentro de <head></head> pero tambien dentro de ```<style></style>``` y se va aplicando el codigo
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
En este caso no se pone en la cabecera si no que se aplica directamente al codigo html dentro del body , usando el atributo style.

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
## 3 CREA UNA LISTA SIN ORDENAR CON 5 INGREDIENTES DE UNA RECETA DE COCINA.

```html
<!DOCTYPE html>
<html>
<head>
	<title>Esteban's Recipe</title>
</head>
<body>
	<ul>
		<p>Arroz con atún</p>
		<li>
			Arroz
		</li>
		<li>
			Aceite de oliva
		</li>
		<li>
			Atún
		</li>
		<li>
			Tomate natural
		</li>
		<li>
			Orégano
		</li>
	</ul>
</body>
</html>
```
## 4 COMO SE PUEDE INCLUIR JAVASCRIPT EN HTML.

### Javascript Externo:
Se pone la direccion donde esta el archivo con el codigo javascript en la cabecera , dentro de ```<head></head>``` y tambien dentro
de ```<script></script>```.

EJEMPLO:
```html
<!DOCTYPE html>
<html>
<head>
  <script type="text/javascript" src="scriptEsteban.js"></script>
</head>
...
```

### Javascript Interno:
De esta forma tambien se pone en la cabecera ,dentro de ```<head></head>``` y tambien dentro de ```<script></script>```
pero con la diferencia que aqui se pone el codigo directamente.


EJEMPLO:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo javascript Interno Esteban</title>
    <script type="text/javascript">
        alert('Hola Manol');
    </script>
</head>
...
```
### Javascript en los elementos:
En este caso no se pone en la cabecera si no que se aplica directamente al codigo html dentro del body , usando el atributo oneclick.

EJEMPLO:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo</title>   
</head>
<body>
  <span onclick="alert('Hola otra vez Manol!')">Haz click aquí</span>
</body>
...
```
