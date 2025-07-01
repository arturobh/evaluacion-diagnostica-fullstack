# 📚 Sección 1 - Fundamentos de JavaScript

## 🧠 Preguntas teóricas

### 1. ¿Cuál es la diferencia entre *hoisting* en `var`, `let` y funciones?
El hoisting es el comportamiento de JS que hace que las declaraciones sean "elevadas" al inicio del contexto de ejecución (scope), sin embargo, se comporta de forma distinta dependiendo del tipo de entidad que se trate:

**Var:**  
La declaración es *"hoisteada"* pero es inicializada como `undefined`
Ejemplo: 
```js
console.log(b); // undefined
var b = 10;
```
**Let y const:**  
La declaración es *"hoisteada"* pero aunque existe, no se puede acceder a ella (Temporal Dead Zone)
Intentar acceder a ella arroja un `ReferenceError`  
Ejemplo:
```js
console.log(a); // ReferenceError: Cannot access 'a' before initialization
let a = 10;
```
**Function declaration:**  
Tanto la declaración como su inicialización son *"hoisteadas"*, ya que al declarar la función se debe asignar su contenido al mismo tiempo  
Ejemplo:
```js
console.log(function_declaration); // [Function: function_declaration] -> Funciona correctamente
function function_declaration() {
    console.log("Function Declaration");
}
```
**Function expression:**  
Únicamente la variable es *"hoisteada"* (si es var), pero no el contenido de la variable (la función en si)  
Se comporta de la misma manera que una variable **var** o **let** / **const**  
Ejemplo: 
```js
console.log(function_expression);  // undefined
var function_expression = function() {
    console.log("Function Expression");
}

console.log(function_expression);  // ReferenceError: Cannot access 'function_expression' before initialization
let function_expression = function() {
    console.log("Function Expression");
}
```

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
