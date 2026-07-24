# Clave de respuestas — Actividad Clase 1 (solo para vos, no para repartir)

## Paso 0
En el `<head>` de `index.html` debe quedar:
```html
<link rel="stylesheet" href="estilos.css">
```
Y en `estilos.css`:
```css
body { background-color: #f0f0f0; }
```

## Nivel 1
```css
h2 { color: #534AB7; }
p  { color: #2C2C2A; }
```
Cualquier color distinto entre `h2` y `p` es válido — lo que importa es que vean que cada etiqueta se estiliza de forma independiente.

## Nivel 2
```css
.destacado { background-color: #FFF3C4; }
```
Chequeá que el color de texto que definieron en `p` (Nivel 1) se siga viendo dentro de `.destacado` — es la prueba de que las reglas se acumulan.

## Nivel 3 — el desafío
```css
p { color: blue; }
.aviso { color: red; }
```
**Resultado esperado: el texto queda rojo**, sin importar el orden en que escriban las dos reglas. `.aviso` es un selector de clase (peso 10) y `p` es un selector de etiqueta (peso 1) — gana el que más pesa, no el que está más abajo.

Si algún alumno dice que "ganó porque estaba después", es la señal de que está aplicando la lógica de la cascada (clase 5 de la planificación general) en un caso donde en realidad decide la especificidad. Vale la pena marcarlo en el momento, no esperar a la clase 7.

## Errores comunes a esperar
- Escribir `.destacado` como `destacado` (sin el punto) — no selecciona nada, buen disparador para recordar la sintaxis.
- Confundir `color` con `background-color` en el Nivel 2.
- En el Nivel 3, probar solo un orden y no invertirlo — sin el paso de invertir, no llegan a comprobar que el orden no importa acá.
