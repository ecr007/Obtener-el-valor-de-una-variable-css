#Get Valor de una variable CSS con JavaScript

```
:root {
  --color-principal: red;
}
 
p {
  color: var(--color-principal);
}
<p>Este párrafo es de color rojo.</p>
var estilosCss = getComputedStyle(document.documentElement);
var valor = String(estilosCss.getPropertyValue('--color-principal')).trim();
// valor = 'red'

```

# Editar el valor de una propiedad

para cambiar el valor de una variable CSS en el propio navegador, utiliza el método setProperty() del objeto CSSStyleDeclaration.

```

:root {
  --color-principal: red;
}
 
p {
  color: var(--color-principal);
}
<p>Este párrafo ahora es de color verde.</p>
document.documentElement.style.setProperty('--color-principal', 'green');

```


#Asignar el valor de una variable a otra con javascript

```

:root {
  --color-principal: red;
  --color-secundario: blue;
}
<p>Y ahora este párrafo es de color azul.</p>
document.documentElement.style.setProperty(
  '--color-principal', 'var(--color-secundario)'
);

```
