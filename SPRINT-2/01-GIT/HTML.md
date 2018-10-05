# HTML
### HyperText Markup Language

Todos nostros alguna vez en nuestra vida hemos interactuado con alguna página web por alguna razón u otra, incluso ahora mismo.

HTML **no es un lenguaje de programación**, es un lenguaje de marcado de hipertexto, básicamente este lenguaje se escribe con elementos como etiquetas, contenido y atributos. Así lo interpreta el navegador web para mostrar los sitios a como estamos acostrumbrados a verlos.

![html](http://blog.embluemail.com/wp-content/uploads/2018/02/diseniook-750x422.png)

Les mostraré las etiquetas más comunes de HTML y para qué se usan:

### <!DOCTYPE html>
En cualquier lugar podemos escribir en html, incluso en un block de notas.
La declaración siempre debe ser la primera línea de código en sus archivos html. Esto le permite al navegador saber qué versión de html esperar.
Para que funcione esto, se usa la etiqueta ***<!DOCTYPE html>***.

### < html> < /html>
Al igual que la primera etiqueta que mostré, esta sirve para identificar el documento de donde a donde pertenece. El elemento HTML contendrá todo su código html.

 `Nota: como has visto, las etiquetas empiezan con <> y terminan en </> ( al menos la mayoría ), esto con el fin de identificar en qué parte de la estructura empezarán los cambios y en qué parte terminarán.`
## < body> </ body>
Representa el contenido del documento. Sólo puede haber un elemento **body** en todo el documento html.
### < head> </ head>
La información sobre la página web, como el título, pertenece al < head> de la página.
Todo lo que va al principio, le pertenece a esta etiqueta.
### < h1> < /h1>
En html para poner un encabezado y su tamaño se usan las siguientes etiquetas:
+ < h1 > < /h1>
+ < h2 > < /h2>
+ < h3 > < /h3>
+ < h4 > < /h4>
+ < h5 > < /h5>
+ < h6 > < /h6>  

Dónde: **h1** es el título más grande y el **h6** para el más pequeño. Aunque también se puede modificar el tamaño de un párrafo en específico con **CSS**.
### < title> < /title>
Puede agregar un título a su página  web utilizando el elemento < title>, dentro del head.
**El título de un página web aparece en la pestaña del navegador.**
~~~
<head>
   <title>Título de la página</title>
</head>
~~~
### < div> </ div>
Sirve para crear secciones o separar contenidos que tal vez no tengan una etiqueta específica y que se pueda separar.
~~~
<div style="color: blue;">
 <h2> Ejemplo de div y span </h2>
  <p>
    Esto es un párrafo dentro de un div,
    <span style="color: red;"> y esto un span dentro de un párrafo.</span>
  </p>
</div>
~~~


### < p> </ p>
Esta etiqueta se refiere a los párrafos, sirve para distribuir el texto en párrafos y esté mejor ordenado o tenga mejor visualización al momento de ver el código.
~~~
<p>
Esto
es un
párrafo
</p>
~~~

### < span> </ span>
span es un elemento de línea, esto quiere decir que sólo en una parte de la línea será aplicada el formato que le queremos agregar, a diferencia de **div** que va dirigido a elementos de bloque.
~~~
<div>
			<p>Párrafo con formato <span style="color: blue">aplicado</span> a un elemento en línea</p>
		</div>
	</body>
</html>
~~~
![Span](https://disenowebakus.net/imagenes/mezcla-div-span-html.jpg)

### < em> </ em>
En html igual se pueden agregar estilos como *italics*, que enfatiza el texto que seleccionamos.
~~~
<body>
 <p>Esto es un ejemplo para <em>enfatizar</em> sólo una parte</p>
</body>
~~~
### < strong> < /strong>
De igual manera se puede **resaltar** el texto importante con esta etiqueta que funciona como **negritas.**
~~~
<body>
 <p>Este ejemplo representa como poner en <bold>negritas</bold> una parte del texto </p>
</body>
~~~

### < br >
Esta etiqueta permite dejar un espacio entre columna o texto, produce un salto de línea. Es útil para escribir un poema o una dirección, donde la división de las líneas es importante, No utilices **<br>** para incrementar el espacio entre líneas de texto; para ello utiliza la propiedad margin de CSS o el elemento **<p>**.
~~~
<p>

  Jon Nieve<br>

  Camino real 1648<br>

  Invernalia, Poniente

</p>
~~~
### < ul> < /ul>  < li> < /li>  < ol> < /ol>
Estas etiquetas sirven para hacer listas ordenadas o desordenadas.  
**Desordenadas:**
+ Cafe
+ Té   
~~~
<ul>
 <li>cafe<li>
 <li>té</li>
</ul>
~~~

**Ordenadas:**
1. Cafe
2. Té

~~~
<ol>
 <li>cafe</li>
 <li>té</li>
</ol>
~~~
### < img>
Claro que en nuestra página no pueden faltar las imágenes para darle mejoras visuales.
Requiere de dos atributos: **src** y **alt**. Las imágenes técnicamente no son insertadas en una página html, las imágenes son vinculadas a las páginas de html. La etiqueta < img> crea un espacio de retención para la imagen a la que hace referencia.  
Se puede hacer que una imagen te mande a otra página, tipo link, pero se necesita de otra etiqueta **<a>**.  
Dónde **src** es el link de la página y **alt** la descripción que le queramos dar.
~~~
<p>
Una imagen que es link:
<a href="https://www.w3schools.com">
<img src="smiley.gif" alt="Click en la imagen para ir al siguiente link!" width="42" height="42" border="0">
</a>
</p>
~~~
![Ejemplo](https://media.giphy.com/media/1fkE3e1tA5KEfJHrbu/giphy.gif)

### < video>
El uso de esta etiqueta es casi igual al de imagen. En ambos casos se puede usar **"width"** y **"height"**
~~~
<video src="https://www.youtube.com/watch?v=ilUCwLLdltQ" width="320" height="240"controls>
</video>
~~~

### < a>
Las etiquetas de anclaje < a> se usan  para vincular páginas internas, páginas externas o contenidos en la mism página. Puede crear secciones e un página web y saltar a ellas usando las etiquetas < a> y agregando identificarodres a los elementos a los que desea saltar.  
El atributo que se usa es **href** y dentro se pone el link.
~~~
<a
 href="https://github.com/PaulaSshun/tatooine/blob/develop/SPRINT-2/01-GIT/README.md">Link a mi perfil!</a>
~~~
### < !--comment-->
 Los comentarios van escritos dentro la etiqueta y no serán mostrados en el navegador
 ~~~
 < !--Esto es un comentario. Los comentarios no serán desplayados en el navegador-->
 ~~~
 ### < table>
 Esta etiqueta sirve para poner tablas, dentro de esta etiqueta existen otras que sirven para ordenar mejor la información:  
 + Table: **< table>** agregar una tabla.
 + Table data: **< td>** agrega datos a una fila.
 + Table row: **< tr>** agrega filas a una tabla.
 + Table heading: **< th>** agrega los títulos de la tabla.   

***Las tablas se pueden dividir en tres secciones principales: una cabeza, un cuerpo y un footer.***  
 + **< thead>:** Cuando se separa el cuerpo de una tabla, también tiene un sentido dividir los encabezados de la tabla. O sea, la cabeza de una tabla.
 + **< tbody>:** Las tablas largas se pueden seccionar utilizando el elemento del cuerpo de la tabla.
 + **< tfoot>:** El pie de página de una tabla se crea con este elemento. Se usan para contener sumas, diferencias y otros resultados de datos.    
~~~
< head> < title>Ejemplo de tabla sencilla</ title></ head>
< body>
< h1>Listado de cursos</ h1>
< table>
< tr>
 < td>< strong> Curso</ strong></ td>
 < td>< strong> Horas</ strong></ td>
 < td>< strong> Horario</s trong></ td>
</ tr>
< tr>
 < td> CSS</td>
 < td> 20</ td>
 < td> 16:00 - 20:00</td>
</ tr>
< tr>
 < td>HTML</ td>
 < td>20</ td>
 < td>16:00 - 20:00</ td>
</ tr>
< tr>
 < td>Dreamweaver</ td>
 < td>60</ td>
 < td>16:00 - 20:00</ td>
</ tr>
<tfoot>
 <tr>
   <th>Total</th>
   <td>100<td/>
  </tr>
<tfoot>
</ table>
</ body>   
~~~
<body>
<h1>Listado de cursos</h1>

<table>
<tr>
  <td><strong>Curso</strong></td>
  <td><strong>Horas</strong></td>
  <td><strong>Horario</strong></td>
</tr>

<tr>
  <td>CSS</td>
  <td>20</td>
  <td>16:00 - 20:00</td>
</tr>

<tr>
  <td>HTML</td>
  <td>20</td>
  <td>16:00 - 20:00</td>
</tr>

<tr>
  <td>Dreamweaver</td>
  <td>60</td>
  <td>16:00 - 20:00</td>
</tr>
<tfoot>
 <tr>
   <th>Total</th>
   <td>100<td/>
  </tr>
<tfoot>
</table>

</body>
##### Colspan y rowspan
1. **Colspan:** Los datos pueden abarcar columnas utilizando el atributo *"colspan"*. Los atributos aceptan un número entero (mayor que o igual a 1) para indicar el número de columnas que abarca.
2. **Spanning rows:** Pueden abarcar varias filas los datos utilizando *rowspan*. Se utiliza para datos que abarcan varias filas (tal vez un evento continúa durante varias horas en un día determinado.) Acepta un número entero (>=1 ) para indicar el número de filas que abarcar.
~~~
<table>
<tr>
 <th></th>
 <th>Sábado</th>
 <th>Domingo</th>
</tr>
<tr>
 <th>Mañana</th>
 <td rowspan="2">trabajo</td>
 <td rowspan="3">descanso</td>
</tr>
<tr>
 <th>tarde</th>
 <td>cena</td>
</tr>
<tr>
<th>Noche</th>
 <td colspan="2">dormir</td>
</table>
~~~
<table>
<tr>
 <th></th>
 <th>Sábado</th>
 <th>Domingo</th>
</tr>
<tr>
 <th>Mañana</th>
 <td rowspan="2">trabajo</td>
 <td rowspan="3">descanso</td>
</tr>
<tr>
 <th>tarde</th>
 <td>cena</td>
</tr>
<tr>
<th>Noche</th>
 <td colspan="2">dormir</td>
</table>
3. **Scope:** indica las celdas para las que esta celda será su cabecera.  
   Ejemplo: **scope="col"** indica que esta celda es la cabecera de todas las demás celdas que están en la misma columna.  
**row**: Este valor deja en claro que el encabezado es para una fila.
~~~
<table>
 <tr>
  <th></th>
  <th scope="col">Sábado</th>
  <th scope="col">Domingo</th>
</tr>
<tr>
 <th scope="row">Temperatura</th>
 <td>78</td>
 <td>81</td>
</tr>
</table>
~~~
<table>
 <tr>
  <th></th>
  <th scope="col">Sábado</th>
  <th scope="col">Domingo</th>
</tr>
<tr>
 <th scope="row">Temperatura</th>
 <td>78</td>
 <td>81</td>
</tr>
</table>
![Tablas](https://image.slidesharecdn.com/5-tablasenhtml-120212220739-phpapp01/95/tema-5-tablas-en-html-5-728.jpg?cb=1329084579)
![Tablas2](https://image.slidesharecdn.com/5-tablasenhtml-120212220739-phpapp01/95/tema-5-tablas-en-html-6-728.jpg?cb=1329084579)

Estas son las etiquetas más usuales en HTML, estás listo para ponerlas en prática.  
`Paula Sshun 2018 ®`
