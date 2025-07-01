# 📚 Sección 1 - Fundamentos de JavaScript

## 🧠 Preguntas teóricas

### 1. ¿Cuál es la diferencia entre *hoisting* en `var`, `let` y funciones?
En los 3 casos el hoisting "eleva" las declaraciones de las variables al inicio, para las variables **let** a diferencia de las **var** el hoisting las deja en una zona muerta (**Time Dead Zone**), en la que un error de referencia a la variable ocurre de todas formas al llamarla antes de la línea de su declaración. Y en cuanto a las funciones, el hoisting eleva tanto la declaración como su inicialización ya que las funciones se declaran e inicializan con su contenido al mismo tiempo.

### 2. Explica el concepto de *event loop* con un ejemplo claro.

### 3. ¿Cómo afecta el uso de `this` dentro de una arrow function vs una función regular?

---

## 💻 Ejercicio práctico

### 🔹 Enunciado:
Implementa una función `memoize(fn)` que almacene resultados anteriores para evitar cálculos repetidos.

### 🔹 Enfoque:
Describe tu estrategia y decisiones.

### 🔹 Código:
```js
// Tu implementación acá
