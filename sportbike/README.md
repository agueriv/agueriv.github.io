# <span style="font-size: 150%; display: flex; justify-content: center;">[PROYECTO CSS: SPORTBIKE](https://agueriv.github.io/)</span>
### <span style="display: flex; justify-content: center; margin-bottom: 1em;">*Sitio web para proyecto de CSS del segundo trimestre*.</span>

---

> ## <span style="color: orange;">Contenido del proyecto</span>

> La página realizada es una página web de una tienda y taller de motocicletas. Cuenta con sección de historia sobre la empresa, un catálogo de todos los productos que ofrecen, una sección de taller donde se especifica lo que hacen, sus horarios y precios, una sección de donde estamos para establece una ubicación con google maps y una sección de contacto donde tenemos un formulario de contacto simple.

---

> ## <span style="color: orange;">Técnica utilizada</span>

> Página Web desarrollada con HTML y CSS básico. No responsive.

---

> ## <span style="color: orange;">Addons no explicados en clase</span>

> ### Efecto Hover Aumento de tamaño
> Este efecto lo realizamos al realizar el hover sobre un elemento. Codificamos que este elemento aumente de tamaño usando un *transform: scale()*
``` html5
elemento:hover {
	transform: scale();
}
```
> ### Importación de Tipografía Personalizada
> Estas fuentes personalizadas las importamos con la sentencia de CSS *font-face* la cual nos permite importarlas desde cualquier url
```
@font-face {
	font-family: 'Tipografia';
	src: url();
}
```
> ### Efecto de movimiento en hover
> Usamos un estilo de css que nos proporciona el movimiento de una capa al hacer hover sobre ella. Para ello usamos la propiedad *transform: translateY()*.
```
elemento:hover {
	transform: translateY();
}
```
> ### Cambio de texto a mayúsculas (text-transform)
> Para asegurarnos de que las letras son mayúsculas y mejorar la estética de los títulos, he utilizado la propiedad *text-transform* para poner a mayúsculas dichas letras.
```
elemento {
	text-transform: uppercase;
}
```
> ### Subrayado animado, underline
> He realizado un efecto hover que realiza un subrayado animado sobre los textos. Esto lo he realizado mediante el pseudoselector :after. Creamos un subrayado que luego dimos animación mediante un hover
```
.underline {
	display: inline-block;
	position: relative;
}
.underline:after {
	content: '';
	position: absolute;
	width: 100%;
	height: 4px;
	bottom: 0;
	left: 0;
	background-color: #f72a2a;
	transform: scaleX(0);
	transform-origin: bottom right;
	transition: transform 0.4s ease-out;
}
.underline:hover:after {
	transform: scaleX(1);
	transform-origin: bottom left;
}
```

---

> ## <span style="color: orange;">Instalación</span>

> 1. Clonamos el repositorio
> 2. Acceder a la carpeta *agueriv.github.io*
> 3. Abrimos el archivo *index.html* en nuestro navegador
> 4. Listo, ya podremos visualizar la página
