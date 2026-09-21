# Planificación de Capacitación

## Tema elegido a realizar en la capacitación  

# Lógica de programación (Las estructuras de control aplicadas a la vida cotidiana)  

## Una lista preliminar de subtemas a desarrollar

### Introducción y Toma de Decisiones Básico  
Condicional simples if “Si se cumple la condición se ejecuta la acción”  
Condicional compuesta if - else o si - entonces  
OPERADORES AND, OR NOT  

### Toma de Decisiones Complejas  
Condicionales anidadas  
El Puente al Switch  
Selección múltiple (Switch/Case)  

### Bucles For, While y Errores de Bucle  
Bucle for  
Bucle while  
Bucle infinito  

### Evaluación Posterior y Flujo Real 
Condición al final (Do-While)  
Manejo de Eventos e Interrupciones   

### Modularización y Conclusión  
Funciones, Modularidad y Ámbito  
Integración de todo en una rutina diaria  
Manejo de Errores y Excepciones 

## Cronograma de duración de cada sección de la capacitación (Rundown)
| Integrante   | Subtema                                  | Contenido                                                                                                                                    | Ejemplos                                                       | Tiempo |
| ------------ | ---------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- | ------ |
| Integrante 1 | Introducción y Toma de Decisiones Básico | •Condicional Simple (If) "Si se cumple la condición Ejecuta acción"• Condicional Compuesta (If - Else) • Mención de operadores (AND/OR/NOT). | Clima (usar abrigo), ir al cine (dinero Y tiempo).             | 12 min |
| Integrante 2 | Toma de Decisiones Compleja              | • Condicionales anidadas.• El Puente al Switch • Selección múltiple (Switch/Case).                                                           | Menú de comida saludable, ascensor/menú de teléfono.           | 12 min |
| Integrante 3 | Repetición y Ciclos (Bucles)             | • Introducción a la Iteración • Bucles contados (For).<br>• Bucles condicionales (While)• Breve mención: "Bucle infinito" (30s).             | Series de gimnasio, masticar la comida, buscar llaves.         | 12 min |
| Integrante 4 | Evaluación Posterior y Flujo Real        | • Condición al final (Do-While).Manejo de Eventos e Interrupciones • Manejo de eventos e interrupciones.                                     | Probar la sazón de la comida, contestar una llamada cocinando. | 12 min |
| Integrante 5 | Modularización y Conclusión              | • Funciones, Modularidad y Ámbito • Integración de todo en una rutina diaria.• Manejo de Errores y Excepciones                               | Dividir la rutina en bloques (mañanas, estudio, ejercicio).    | 12 min |


## Perfil de la audiencia y estrategia de adaptación del mensaje  

Todo el material utilizado en el video de la planificación el material que no se encuentre en el documento no será tomado como válido

## Estructura de la Capacitación

# CONTENIDO QUE SE PRESENTARRA EN LA CAPACITACIÓN

**Tema:** Lógica de programación: estructuras de control aplicadas a la vida cotidiana
**Duración:** 60 minutos

---

## 1. Introducción

- La lógica de programación no es exclusiva de las computadoras: es una forma estructurada, paso a paso, de resolver problemas.
- El cerebro ejecuta "algoritmos" de forma automática para decidir, repetir tareas y reaccionar al entorno.
- Temas a cubrir: toma de decisiones (simple y compleja), repeticiones y bucles, flujo de ejecución y modularidad.

---

## 2. Toma de decisiones básica

### 2.1 Condicional simple `if`
- Evalúa una condición y ejecuta un bloque **solo si es verdadera**. Si es falsa, lo omite y sigue con la siguiente línea.
- Es una estructura de "todo o nada".
- **Ejemplo:** cajero de estacionamiento. Si el cupón es "DESCUENTO20", se resta el 20%; si no, se muestra la tarifa regular.

### 2.2 Condicional compuesto `if-else`
- Ofrece **dos caminos mutuamente excluyentes**, así que siempre ocurre algo: acción A si es verdadera, acción B si es falsa.
- **Ejemplo:** acceso a un sitio web según la edad (≥ 18 entra, si no, se deniega).

### 2.3 Operadores lógicos

| Operador | Regla | Ejemplo cotidiano |
|---|---|---|
| **AND** | Todas las condiciones deben ser verdaderas | Levantarse si ya amaneció **y** es día laboral |
| **OR** | Basta con que una sea verdadera | Entrar al edificio si tienes identificación **o** estás en la lista de visitantes |
| **NOT** | Invierte el valor lógico | "Hoy hace frío" → "Hoy **no** hace frío" |

---

## 3. Toma de decisiones complejas

- Permite que el software deje de ser lineal y se adapte. Los problemas reales rara vez se reducen a una sola pregunta.
- Surge por dos razones:
  - **Dependencias jerárquicas:** una acción exige requisitos previos en cadena.
  - **Múltiples caminos categóricos:** una variable puede tomar muchos valores distintos.
- **Reto del programador:** legibilidad frente a funcionalidad. El código debe ser mantenible y escalable, sin errores lógicos difíciles de depurar.

### 3.1 Condicionales anidadas (complejidad jerárquica)
- Un `if`/`else` dentro de otro bloque condicional. Crea una dimensión vertical, no solo horizontal.
- **Primera barrera (externa):** regla general de alta prioridad. Si falla, se ignora todo el bloque interno.
- **Segunda barrera (interna):** detalles o subcategorías, solo si la externa se cumple.
- **Ejemplo:** acceso al laboratorio. Si está matriculado, entonces si tiene carné activo, entonces si hay cupos, se permite el acceso; si no, se deniega con un mensaje distinto en cada nivel.
- **Riesgo:** el "código en pirámide", que pierde legibilidad y genera deuda técnica.

### 3.2 El puente al Switch
- **Problema:** una cadena larga de `else if` para un menú (ver notas, modificar perfil, inscribir cursos, consultar laboratorios, salir).
- **Fallas de la cadena:** redundancia sintáctica (viola DRY), baja legibilidad y mantenimiento complejo, y evaluación secuencial O(n).
- **Cambio de mentalidad:** pasar de preguntar "¿se cumple esta condición compleja?" a preguntar "¿qué valor exacto tiene esta variable?".

### 3.3 Selección múltiple `switch/case` (complejidad categórica)
- Evalúa **una sola expresión** contra valores constantes predefinidos, como un "distribuidor de tránsito".
- **Cuatro elementos:**
  1. `switch`: la expresión evaluada.
  2. `case`: cada valor exacto posible.
  3. `break`: sale del switch al terminar el caso.
  4. `default`: red de seguridad, equivalente al último `else`.
- **Peligro oculto (fall-through):** sin `break`, la ejecución "cae" al siguiente caso.
- **Ejemplo:** el menú universitario resuelto con `switch`.
- **Ventajas:** mejor legibilidad y mantenimiento, y posible optimización del compilador con tablas de saltos.
- **Regla de oro:** solo sirve para valores discretos exactos. Para rangos (nota entre 61 y 100) se usa `if`.

---

## 4. Repetición o ciclos

- Permiten ejecutar instrucciones varias veces sin reescribirlas.
- **Flujo general:** inicio → evaluación → ejecución → actualización → nueva evaluación → repetición o fin.

### 4.1 Ciclo `for` (repetición controlada)
- Pregunta clave: **¿cuántas veces necesito repetir esto?**
- Partes: inicialización, condición o límite, actualización.
- **Ejemplo:** escribir "Hola" 5 veces.
- **Vida cotidiana:** hacer 10 ejercicios, dar 3 vueltas a la cancha.

### 4.2 Ciclo `while` (repetición basada en una condición)
- Pregunta clave: **¿hasta cuándo necesito repetir esto?**
- **Ejemplo:** imprimir del 1 al 5 con `numero = numero + 1`.
- **Vida cotidiana:** estudiar mientras haya tareas pendientes, atender una fila.

### 4.3 Diferencia `for` vs `while`

| `for` | `while` |
|---|---|
| Cantidad de repeticiones conocida o controlada | Repetición basada en una condición |
| Usa un contador | Usa una condición |
| "Repetir 10 veces" | "Repetir mientras se cumpla algo" |

### 4.4 Ciclo infinito
- Un ciclo que nunca termina porque la condición siempre se cumple (por ejemplo, olvidar actualizar `numero`).
- Pregunta de diseño: **¿qué hará que este ciclo termine?**

### 4.5 Importancia de los ciclos
- Reducen código, evitan instrucciones repetidas, procesan grandes cantidades de información, automatizan tareas y mantienen los programas organizados.

### 4.6 Ciclo `do-while` (evaluación posterior)
- Ejecuta el bloque **al menos una vez** y evalúa la condición después. Filosofía: "haz la acción primero y pregunta después".
- **Analogía:** la pizza. Te comes el primer trozo y luego te preguntan si quieres otro.
- **Diferencia con `while`:** `while` revisa primero, y si la condición es falsa, ni arranca.
- **Usos reales:** menús principales de apps o videojuegos y sistemas de autenticación o cajeros.
- **Importancia:** garantiza la ejecución y evita repetir código en menús o pantallas de bienvenida.

---

## 5. Manejo de eventos e interrupciones

- **Analogía:** estás jugando o viendo una serie y suena el timbre. Pausas, atiendes y retomas donde te quedaste.
- **Evento:** estímulo externo que el software espera para reaccionar (clic, toque, tecla, sensor). Es la base de la Programación Orientada a Eventos.
- **Interrupción:** evento de alta prioridad que obliga al procesador a suspender su tarea, atender la emergencia y luego regresar.
- **Ejemplos cotidianos:** pantalla táctil (evento), teclado (interrupción) y microondas que se detiene al abrir la puerta (interrupción física).
- **Importancia:**
  - Eventos: interactividad y conexión usuario-máquina en tiempo real.
  - Interrupciones: eficiencia del procesador, atención a emergencias, seguridad y rapidez.
- **Conexión final:** un software interactivo integra `do-while` para mantener el programa activo, eventos para la interacción y un sistema de interrupciones para las pausas y tareas críticas.

---

## 6. Funciones, modularidad y ámbito

### 6.1 Funciones
- Bloque de código con nombre que agrupa instrucciones y se puede llamar cuantas veces se quiera sin reescribirlo.
- **Analogía:** la máquina de café. Solo pides "café" y ella ya sabe moler, calentar y mezclar.

### 6.2 Modularidad
- Dividir algo grande en partes pequeñas, cada una con su propia tarea, que se revisan y corrigen por separado.
- **Analogía:** los sistemas del cuerpo humano (digestivo, respiratorio, circulatorio). Si uno falla, no se "rediseña" a toda la persona.

### 6.3 Ámbito (scope)
- Define qué información es privada de una parte del programa y cuál puede usar todo el sistema.
- **Analogía:** el cuaderno personal (**local**) frente al pizarrón del salón (**global**).
- Mezclar mal ambos genera problemas.

---

## 7. Síntesis y cierre

- **Mensaje central:** no se enseña algo nuevo, sino que se le pone nombre a lo que ya hacemos todos los días.
- Elegir la ropa según el clima es un `if-else`, repetir un hábito es un `for` o `while`, atender una interrupción y volver a lo que hacíamos es un evento, y una acción automática es una función.
- La programación es una forma de escribir con reglas claras la lógica que ya usamos para vivir.
- Se agradece la atención y se abre la sesión de preguntas.

---

## 8. Actividades y dinámicas

### 8.1 Actividad 1: "El Robot en su Asiento"
- El capacitador actúa como un robot sin sentido común que solo ejecuta instrucciones literales.
- Los estudiantes deben darle instrucciones para **sacar su cuaderno de la mochila y abrirlo en una página limpia**.
- El robot falla ante instrucciones ambiguas o incompletas (mochila cerrada, objeto no especificado, página no indicada).
- **Objetivo:** mostrar que un algoritmo necesita pasos precisos, ordenados y sin ambigüedad.

### 8.2 Actividad 2 : "Identifica la estructura"
Los participantes responden con dedos: 1 = secuencia, 2 = condicional, 3 = bucle.

| Situación | Respuesta |
|---|---|
| Preparar cereal con leche (plato, cereal, leche) | 1 dedo, secuencia |
| Mirar por la ventana: si llueve, sombrilla; si no, lentes de sol | 2 dedos, condicional |
| Alarma que se pospone cada 5 min hasta que te levantas | 3 dedos, bucle |

### 8.3 Preguntas para la audiencia Y PREMIOS
- SI RESPONDEN CORRECTAMENTE LOS ESTUDIANTES Y COLABORAN RECIBEN PREMIOS

| Responsable | Pregunta |
|---|---|
| Hassan | ¿La toma de decisiones simple requiere que una condición sea verdadera para cumplirse, o puede no serlo y cumplirse? |
| Carlos | Sistema de notas (61-100 aprueba): ¿se puede usar `switch` o se está obligado a usar `if`? ¿Por qué? |
| Naomi | Si se repite una acción exactamente 10 veces, ¿qué ciclo se usa, `for` o `while`, y por qué? |
| Dennis | Para ejecutar una acción al menos una vez antes de evaluar condiciones, ¿`while` o `do-while`? |
| Aimar | Dinámica "Encuentro tu número", trabajo en conjunto con un condicional `if-else` |
