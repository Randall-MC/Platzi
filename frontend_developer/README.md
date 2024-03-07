# Curso de Frontend Developer

Domina las bases de HTML y CSS. Conoce la anatomía de un documento HTML, sus elementos y las propiedades de CSS. Maqueta las pantallas principales de tu página web con responsive design. ¡Conviértete en Frontend Developer con Platzi!

> Estefany Aguilar  
> Desarrolladora Frontend en Platzi

---

## Notas del curso

### HTML Semántico

Utiliza etiquetas con significado siempre que sea posible. No es una buena práctica usar `<div>` para agrupar elementos. Algunas ventajas de usar etiquetas semánticas son:

- Ayuda a tu sitio a ser accesible
- Mejora tu posicionamiento SEO
- Código más claro

[Aquí](https://htmlreference.io/) una página donde encontrarás una guía de HTML

[Aquí](https://htmlcolorcodes.com/es/nombres-de-los-colores/) una página donde encontrarás los códigos de los colores de HTML

### Tipos de selectores

Referencias: [Selectores en CSS](https://developer.mozilla.org/es/docs/Learn/CSS/Building_blocks/Selectors)

**Selectores de tipo** seleccionan todos los elementos del tipo dado dentro de un documento.

```css
/* Selecciona todos los elementos a */
a {
    color: red;
}
```

**Selector universal** coincide con elementos de cualquier tipo.

```css
/* Selecciona todos los elementos */
* {
    color: green;
}
```

**Selectores de clase** buscan un elemento basado en el contenido de su atributo `class`.

```css
span.classy {
    background-color: DodgerBlue;
}
```

**Selectores de ID** buscan un elemento basado en el contenido del atributo `id`.

```css
#demo {
    border: red 2px solid;
}
```

**Selectores de atributo** coincide con los elementos en función de la presencia o el valor de un atributo determinado.

```css
/* Elementos <a> con el atributo title */
a{title} {
    color: purple;
}

/* Elementos <a> con un href que coincida con "https://example.org" */
a[href="https://example.org"] {
    color: green;
}

/* Elementos <a> con un href que contenga "example" */
a[href*="example"] {
    font-size: 2em;
}

/* Elementos <a> con un href que comience con "#" */
a[href^="#"] {
  color: #001978;
}

/* Elementos <a> con un href que termine en ".org" */
a[href$=".org"] {
  font-style: italic;
}

/* Elementos <a> cuyo atributo class contenga la palabra "logo" */
a[class~="logo"] {
  padding: 2px;
}
```

Las pseudo-clases, junto con los pseudo-elementos, permiten aplicar un estilo a un elemento no sólo en relación con el contenido del árbol del documento, sino también en relación a factores externos como el historial del navegador (`:visited` por ejemplo), el estado de su contenido (como `:checked` en algunos elementos de formulario), o la posición del ratón (como `:hover` que permite saber si el ratón está encima de un elemento o no)

**Pseudo-classes** son palabras clave que se añaden a los selectores y que especifica un estado especial del elemento seleccionado.

```css
/* :hover aplicará un estilo cuando el usuario haga hover sobre el elemento especificado por el selector */
div:hover {
    background-color: #F89B4D;
}
```

**Pseudo-elementos** se añaden a los selectores, pero en cambio, no describen un estado especial sino que, permiten añadir estilos a una parte concreta del documento.

```css
/* ::first-line selecciona solo la primera línea del elemento especificado por el selector */
p::first-line {
    color: red;
}
```

**Selectores descendientes** combina dos selectores de forma que los elementos seleccionados por el segundo selector se seleccionan si tienen un elemento antepasado (padre, padre del padre, padre del padre del padre, etc. 🤣😁) que coincida con el primer selector.

```css
/* Selecciona los elementos li de la lista my-things */
ul.my-things li {
    margin: 2em;
}
```

**Selectores de hijo** busca solo a los elementos que coinciden con el segundo selector y que son **hijos directos** del primero. La expresión busca elementos que coinciden con el segundo selector y que tienen un ancestro que coincide con el primero, sin importar el nivel de separación que tenga dentro del DOM.

```css
div > span {
    background-color: DodgerBlue;
}
```

**Selector de hermanos adyacentes**, selector adyacente, o selector del próximo hermano. Sólo seleccionará un elemento especificado que esté inmediatamente después de otro elemento especificado.

```css
li:first-of-type + li {
    color: red;
}
```

**Selector de hermanos generales** selecciona el segundo elemento sólo si está precedido por el primero y ambos comparten un padre común.

```css
p ~ span {
    color: red;
}
```

En [este enlace](https://specificity.keegan.st/) podrás calcular la especificidad de los selectores en CSS.

El posicionamiento en CSS es una de las cosas más importantes. CSS cuenta con herramientas como Flexbox y Grid para que esa tarea sea más fácil. Por lo que dejaré una guía de cada uno.  
[Guía Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
[Guía Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
