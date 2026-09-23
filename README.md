# taller-integrador-vargasaguas

# Calculadora de Promedio — Corrección y despliegue

**Curso:** Buenas Prácticas de Desarrollo de Software
**Universidad:** Corporación Universidad de la Costa
**Estudiante:** Mateo David Vargas Aguas
**Grupo:** 24512

---

## Enlaces del proyecto

| Recurso | Enlace |
|---|---|
| Repositorio | github.com/mateodavidaguas-byte/taller-integrador-vargasaguas |
| Sitio en producción | https://remarkable-rugelach-b39ef9.netlify.app |

---

## Bitácora de auditoría

Al revisar el archivo entregado (`Mi Pagina De Notas.HTML` y `Estilos Del Sitio.CSS`) se encontraron nueve puntos que se alejaban de las buenas prácticas trabajadas en clase. A continuación el detalle de cada uno y cómo quedó resuelto en el commit correspondiente.

**Convenciones de nombres de archivo.** Los archivos originales usaban espacios y combinaban mayúsculas y minúsculas de forma inconsistente, lo cual complica su referencia en rutas y enlaces. Pasaron a llamarse `index.html` y `styles.css`.

**Título del documento.** La pestaña del navegador mostraba únicamente "pagina", un texto que no le dice nada al usuario sobre el contenido. Ahora aparece "Calculadora de Promedio".

**Variable no utilizada.** El script declaraba `data1` sin que ninguna parte del código la referenciara después; se trataba de un residuo del desarrollo. Se quitó por completo.

**Valor numérico sin explicación.** La cantidad de notas (3) estaba escrita directamente como el número mágico `x`, sin contexto de qué representaba. Se convirtió en la constante `CANTIDAD_NOTAS`.

**Nombres de variable ambiguos.** Identificadores como `a`, `b`, `c` y `TempValue2` no comunican su contenido y obligan a rastrear el código para entenderlos. Se cambiaron por `nota1`, `nota2`, `nota3` y `promedio`.

**Identificadores del DOM poco claros.** Los `id` del HTML (`n1`, `n2`, `n3`, `r`, `r2`) tampoco eran autoexplicativos. Quedaron como `notaUno`, `notaDos`, `notaTres`, `resultadoPromedio` y `resultadoEstado`.

**Nombre de función genérico.** `calc()` no deja claro qué calcula la función a simple vista. Se renombró a `calcularPromedio()`.

**Trazas de depuración.** El script conservaba varios `console.log()` usados durante el desarrollo, que no deberían llegar a producción. Se eliminaron todos.

**Fragmento de código inactivo.** Había una función completa (`calcularAntiguo`) comentada, sin uso ni referencia. Se eliminó junto con su comentario.