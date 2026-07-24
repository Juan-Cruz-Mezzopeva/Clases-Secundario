# Clave de respuestas — Actividad Clase 2 (solo para vos)

## Nivel 1 — Padding
```css
.caja-padding { padding: 20px; }
```
Cualquier valor visible (≥10px) es válido — lo que importa es que el texto se despegue del contorno de referencia.

## Nivel 2 — Border
```css
.caja-border { border: 3px solid #534AB7; }
```
Cualquier combinación de grosor/estilo/color es válida.

## Nivel 3 — Margin
```css
.caja-margin-a { margin-right: 20px; }
```
También es válido si ponen `margin` (los 4 lados) en vez de solo `margin-right` — van a ver el mismo efecto entre A y B, aunque también empuje a la caja A respecto de lo que esté a su izquierda.

## Nivel 4 — box-sizing
```css
.caja-ancho {
  width: 200px;
  padding: 20px;
  border: 5px solid #534AB7;
  box-sizing: border-box;
}
```
**Antes de agregar `box-sizing`:** el ancho real es 200 + 20×2 + 5×2 = **250px** — por eso el borde derecho se pasa 50px de la línea dorada.
**Después de agregarlo:** el ancho real vuelve a ser exactamente 200px, y el borde coincide con la línea.

## Nivel 5 — Margen colapsado
```css
.caja-colapso-a { margin-bottom: 30px; }
.caja-colapso-b { margin-top: 30px; }
```
**Resultado esperado sin padding:** el espacio entre las cajas es **30px** (colapsan y se quedan con el mayor de los dos, no 60px).
**Al agregar `padding-bottom: 1px` a la Caja A:** el espacio final pasa a ser **31px** (30px de margin-bottom de B + 1px de padding de A) — porque ahora hay un padding entre medio y los márgenes ya no se tocan directamente, así que dejan de colapsar.

Este último paso es el que más cuesta ver — si algún grupo no nota el cambio de 30 a 31px, sugeriles que midan con la regla del navegador (clic derecho → Inspeccionar → Computed) en vez de calcular a ojo.

## Nivel 6 — Integración
Ejemplo de solución completa:
```css
.tarjeta-final {
  padding: 18px;
  border: 2px solid #0F6E56;
  margin: 20px 0;
  width: 320px;
  box-sizing: border-box;
  background-color: #FFF3C4;
}
```
No hay una única respuesta correcta — lo que hay que revisar es que estén las 6 propiedades pedidas y que el resultado se vea coherente (que el padding no rompa el ancho, por ejemplo).

## Errores comunes a esperar
- En el Nivel 4, agregar `box-sizing: border-box` pero olvidarse de que también hay que dejarlo puesto para que el ancho cierre — a veces lo prueban, lo sacan para "comparar" y se olvidan de volver a ponerlo.
- En el Nivel 5, no notar la diferencia de 1px entre el resultado con y sin padding — es sutil a propósito, para que valoren medir en vez de asumir.
- En el Nivel 6, olvidarse `box-sizing: border-box` y que el ancho final no coincida con lo que esperaban — es la integración de los dos aprendizajes de la clase, vale la pena señalarlo si pasa.
