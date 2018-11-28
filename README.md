# LM

Lenguaje de marcas HTML y CSS

## 1- ESTRUCTURA MINIMA DE UNA WEB.
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
## 2- EXPLICA LAS 3 FORMAS DE USAR CSS EN HTML.

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
## 3- CREA UNA LISTA SIN ORDENAR CON 5 INGREDIENTES DE UNA RECETA DE COCINA.

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
## 4- COMO SE PUEDE INCLUIR JAVASCRIPT EN HTML.

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

## 5- ¿QUE DIFERENCIA HAY ENTRE UNA CLASE Y UNA ID?.


La principal diferencia es que un ID es un identificador único. Es decir que si por ejemplo tienesun ID ejemploEsteban, a ese ID lo vas a utilizar en un solo elemento de html .Los IDs tienen que ser unicos y serán usados en un solo elemento html. Pueden haber muchos IDs, pero cada uno será utilizado una única vez.Mientras que las CLASES se pueden utilizar cuantas veces se quiera y en distintos elementos html.

EJEMPLOS:
```
<div class="esteban">
  <p>Ejemplo de clase</p>	     // Para seleccionarlo hay que poner un punto y a continuacion el nombre por ejemplo : .esteban
</div>
```
```
<h1 id="narajo">Ejemplo de ID</h1> // Para seleccionarlo hay que poner un almohadilla y a continuacion el nombre por ejemplo : #naranjo
```

## 6- CODIGO PARA HACER UN ENLACE A OTRA PAGINA Y QUE ESTA SE ABRA EN UNA VENTANA NUEVA.

```html
<!DOCTYPE html>
<html>
<head>
	<title>EstebanNH</title>
</head>
<body>
	<a href="http://blog.elinsti.com/" target="_blank">web lenguaje de marcas</a>
</body>
</html>
```

## 7- ¿QUE SON LAS PSEUDOCLASES?,pon ejemplos.
Una pseudoclase es una palabra clave que se le añade a los selectores para especificar un estado especial de determinado elemento.

EJEMPLOS:
```
a:active	 //Selecciona cualquier <a> que esté siendo activada

p:hover {
  color: orange; //Cada p , cuando se pose el ratón por encima se colorea de naranja.
}

a:link {
  color: red;   //Selecciona cualquier <a> aunque no se haya visitado.
}
```
## 8- EXPLICA EL MODELO DE CAJA DE CSS (MARGIN,BORDER,PADDING).

### MARGIN:
El margen es el margen que habra en la caja y el resto de cajas. Si se usa solo margin
se cambiaran los cuatro lados de la caja por separado se usan  margin-top, margin-right, margin-bottom, y margin-left.

### BORDER:
Este atributo es obviamente el borde de la caja y se puede dificar el color , el grosor etc.. Al igual que margin si se usa solo border
se cambiaran los cuatro lados de la caja por separado se usan border-top, border-right, border-bottom, border-left.

### PADDING:
Padding hace referencia al margen interior de la caja.Al igual que margin y border si se usa solo la propiedad padding se cambiaran los cuatro lados, y para cada lado por separado se usaran las propiedades padding-top, padding-right, padding-bottom y padding-left.

IMAGEN EJEMPLO: https://mdn.mozillademos.org/files/13647/box-model-standard-small.png

## 9- EXPLICA QUE SON LOS SELECTORES DE CSS Y PON EJEMPLOS.

Los selectores son los que nos permiten elegir los nelementos a los que queremos aplicar unas reglas de diseño. Asi es como podemos dar estilo a todos los elementos HTML que queramos.

EJEMPLOS:
```
p * {
    color: red; // Se selecciona a todas las p del codigo.
}

h1 {
    color: red; // Se selecciona a todOs los h1 del codigo.
}

#principal {
    color: red; // Se selecciona a la ID con el nombre "principal".
}

.esteban {
    color: red; // Se selecciona a todas las clases con el nombre "esteban".
}
```
## 10- DI A QUIEN AFECTA.
```
p a { color: red;  					//Ninguno porque falta cerrar llaves.
p > a { color: red; }					//Afecta a todas las a que sean hijos directos de p.
h1 + h2 { color: red }					//Afecta tanto a los h1 como a los h2 de la pagina.
a[class] { color: blue; }				//Afecta a todas las a que esten dentro una clase.
a[class="externo"] { color: blue; }			//Afecta a todas las a que esten dentro de la clase "externo".
a[href="http://www.ejemplo.com"] { color: blue; }	//Afecta a la a que hace referencia a la url http://www.ejemplo.com
```

# ESTEBAN NARANJO HENRIQUEZ 27/11/2018
