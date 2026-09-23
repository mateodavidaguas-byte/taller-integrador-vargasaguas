# taller-integrador-vargasaguas

# Calculadora de Promedio — Taller Integrador

**Curso:** Buenas Prácticas de Desarrollo de Software
**Universidad:** Corporación Universidad de la Costa
**Estudiante:** [Tu nombre completo]
**Grupo:** [Tu grupo]

---

## 🔗 Enlaces

- **Repositorio:** github.com/mateodavidaguas-byte/taller-integrador-vargasaguas
- **Sitio publicado:** https://remarkable-rugelach-b39ef9.netlify.app

---

## 📋 Hallazgos de la auditoría

### 1. Nombres de archivo
**Problema:** `Mi Pagina De Notas.HTML` y `Estilos Del Sitio.CSS` tenían espacios y mayúsculas, sin seguir la convención de archivos web.
**Solución:** Renombrados a `index.html` y `styles.css`.

### 2. Título de la pestaña
**Problema:** El `<title>` decía simplemente "pagina", sin describir el contenido.
**Solución:** Cambiado a "Calculadora de Promedio".

### 3. Variable sin uso
**Problema:** `data1` estaba declarada pero nunca se usaba en ninguna parte del código.
**Solución:** Eliminada.

### 4. Nombres de variable poco descriptivos
**Problema:** `x`, `a`, `b`, `c` y `TempValue2` no indicaban qué almacenaban, obligando a leer todo el código para entenderlo.
**Solución:** Renombradas a `CANTIDAD_NOTAS`, `nota1`, `nota2`, `nota3` y `promedio`.

### 5. IDs de HTML poco descriptivos
**Problema:** `n1`, `n2`, `n3`, `r` y `r2` no dejaban claro qué elemento representaban.
**Solución:** Renombrados a `notaUno`, `notaDos`, `notaTres`, `resultadoPromedio` y `resultadoEstado`.

### 6. Nombre de función poco descriptivo
**Problema:** `calc()` no indicaba qué hacía la función.
**Solución:** Renombrada a `calcularPromedio()`.

### 7. Código de depuración
**Problema:** Varios `console.log()` quedaron en el código de producción.
**Solución:** Eliminados.

### 8. Código comentado sin uso
**Problema:** La función `calcularAntiguo` estaba comentada y sin ningún propósito.
**Solución:** Eliminada.