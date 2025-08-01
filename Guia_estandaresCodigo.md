# 📘 Guía de Estándares de Codificación – Proyecto Revolución Solar

## Reglas de nombres:

- Variables y funciones en `camelCase` (ej: `obtenerUsuario`)
- Clases en `PascalCase` (ej: `UsuarioRegistrado`)
- Constantes en `MAYÚSCULAS_CON_GUIONES` (ej: `API_URL_BASE`)

---

## Comentarios y documentación:

- Se recomienda el uso de comentarios descriptivos sobre bloques de lógica compleja.
- Se evita comentar lo obvio y se fomenta explicar el propósito del código más que el “cómo”.

---

## Identación y estilo de código:

- Identación de **2 espacios por nivel**.
- Comillas dobles para cadenas (`" "`).
- Uso obligatorio de **punto y coma** al final de cada instrucción.
- Longitud máxima de línea: **80 caracteres**.
- Comparaciones estrictas (`===`, `!==`).
- Uso de `const` y `let` según el contexto.
- Prohibido el uso de `var`.

---

## Ejemplos aceptados y no aceptados:

🧾 Ejemplo tomado de la guía:

```js
// ✅ Aceptado
const nombre = "Juan";
function autenticar(usuario) {
  if (usuario && usuario.rol === "admin") {
    console.log("Autenticado");
  }
}
