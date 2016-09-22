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
