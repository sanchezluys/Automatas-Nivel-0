#### 🌐 Introducción

<img src="0_Introduccion/meet_1.png" alt="meet"	style="height: 600px; margin: 0 auto 4rem auto; background: transparent; box-shadow: 0 0 10px 10px rgb(150, 156, 238); border-radius: 20px;">

---

#### 🎯 Objetivos

<p class="fragment" data-fragment-index="1" style="text-align: left;">
  1. <strong>🧠 Modelos de Computación</strong>: Comprender la base de los autómatas como modelos abstractos de computación.
</p>
<p class="fragment" data-fragment-index="2" style="text-align: left;">
  2. <strong>⚙️ Autómatas Finitos</strong>: Diseñar y analizar Autómatas Finitos Deterministas (AFD) y No Deterministas (AFN).
</p>
<p class="fragment" data-fragment-index="3" style="text-align: left;">
  3. <strong>📝 Expresiones Regulares</strong>: Convertir expresiones regulares a autómatas y viceversa.
</p>
<p class="fragment" data-fragment-index="4" style="text-align: left;">
  4. <strong>🔀 Conversiones y Minimización</strong>: Convertir AFN a AFD y minimizar AFDs para optimizar su eficiencia.
</p>
<p class="fragment" data-fragment-index="5" style="text-align: left;">
  5. <strong>📜 Lenguajes Formales</strong>: Clasificar lenguajes formales según la Jerarquía de Chomsky.
</p>
<p class="fragment" data-fragment-index="6" style="text-align: left;">
  6. <strong>🧪 Aplicaciones Prácticas</strong>: Explorar aplicaciones de autómatas en compiladores, búsqueda de patrones y otras áreas.
</p>

---

#### ⏳ Meta Final: Proyecto de Autómatas en GitHub

<img src="0_Introduccion/plc.jpg" alt="automatas"	style="height: 600px; margin: 0 auto 4rem auto; background: transparent; box-shadow: 0 0 10px 10px rgb(150, 156, 238); border-radius: 20px;" class="demo-logo">

---

#### 🛠️ Requisitos 1/2

<p class="fragment" data-fragment-index="1" style="text-align: left;">
  1. <strong>💻 Entorno de Desarrollo</strong>: IDE o editor de texto con soporte para programación y visualización de autómatas.
</p>
<p class="fragment" data-fragment-index="2" style="text-align: left;">
  2. <strong>🌐 Conexión a Internet</strong>: Necesaria para acceder a documentación, simuladores online y colaborar en GitHub.
</p>
<p class="fragment" data-fragment-index="3" style="text-align: left;">
  3. <strong>🐍 Lenguaje de Programación (Opcional)</strong>: Conocimientos básicos de Python, Java o similar para implementar autómatas.
</p>
<p class="fragment" data-fragment-index="4" style="text-align: left;">
  4. <strong>🧰 Herramientas de Visualización</strong>:  Software o bibliotecas para crear diagramas de estados claros y comprensibles (e.g., Graphviz, Mermaid.js).
</p>

---

#### 🛠️ Requisitos 2/2

<p class="fragment" data-fragment-index="5" style="text-align: left;">
  5. <strong>🌐 GitHub</strong>: Plataforma para versionar, compartir y colaborar en el proyecto de autómatas.
</p>
<p class="fragment" data-fragment-index="6" style="text-align: left;">
  6. <strong>🧑‍🤝‍🧑 Colaboración (Opcional)</strong>: Habilidad para trabajar en equipo si el proyecto es colaborativo.
</p>
<p class="fragment" data-fragment-index="7" style="text-align: left;">
  7. <strong>🧪 Enfoque de Pruebas</strong>: Metodología para verificar el correcto funcionamiento del autómata diseñado (e.g., pruebas unitarias).
</p>
<p class="fragment" data-fragment-index="8" style="text-align: left;">
  8. <strong>📚 Ganas de aprender</strong>: Actitud proactiva para explorar la teoría y práctica de los autómatas.
</p>

===

#### 🚀 Introducción a un Autómata

<img src="0_Introduccion/receta.webp" alt="vista 1"	style="height: 600px; margin: 0 auto 4rem auto; background: transparent; box-shadow: 0 0 10px 10px rgb(150, 156, 238); border-radius: 20px;" class="demo-logo">

---

#### 1. Introducción: ¿Qué son los Autómatas? 🤖

##### ¿Qué es un Autómata? (La Receta Secreta de las Máquinas ⚙️)

> Un autómata es como una receta 📜, un conjunto de instrucciones que una máquina sigue para procesar información.

*   **Analogía 1: El Robot de Cocina 🧑‍🍳:** Imagina un robot que solo sabe hacer sándwiches. La receta (orden de poner pan, jamón, queso...) es el autómata.
*   **Analogía 2: El Detector de Metales 探知機:** Cuando pasas un detector de metales, está buscando un patrón (metal 🪙). Si lo encuentra, "acepta" (hace ruido 🔔). Si no, "rechaza" (se queda callado 🔇).

---

##### ¿Por qué son importantes los Autómatas? (¡Están en todas partes! 🌍)

*   **Ejemplo 1: Asistentes Virtuales (Siri, Alexa 🗣️):** Entienden tus comandos gracias a autómatas que reconocen patrones en tu voz.
*   **Ejemplo 2: Validar Emails ✅:** Cuando te dicen que tu email es inválido ❌, un autómata revisó si tiene el formato correcto (algo@algo.com).
*   **Ejemplo 3: Videojuegos 🎮:** La inteligencia artificial básica de los enemigos (patrullar 🚶, atacar ⚔️) usa autómatas.

---

##### Ejercicio Práctico (¡Piensa como una Máquina! 🤔):

Imagina que eres un autómata que debe decidir si una puerta automática se abre o no. La entrada es si alguien se acerca ("acercar") o se aleja ("alejar"). ¿Qué reglas (transiciones) seguirías?


##### Caso Práctico (La Puerta Automática 🚪):

Dibuja un diagrama simple (a mano alzada ✍️) que represente la puerta automática. ¿Cuáles son los estados (abierta 🔓, cerrada 🔒)? ¿Cuáles son las transiciones?

===

#### 2. Conceptos Fundamentales 📚

##### Alfabeto (Σ): Las Letras del Juego 🔤

> El alfabeto es el conjunto de todos los símbolos que el autómata puede "entender" 🧠.

*   **Definición:** Un conjunto finito de símbolos.
*   **Ejemplo 1: Binario:** Σ = {0, 1} (solo ceros y unos)
*   **Ejemplo 2: Letras:** Σ = {a, b, c, ..., z} (todas las letras del alfabeto 🇦🇧🇨)
*   **Ejemplo 3: Semáforo:** Σ = {🔴, 🟡, 🟢} (rojo, amarillo, verde)

---

##### Cadena (String): La Palabra Secreta 🔑

> Una cadena es una secuencia de símbolos del alfabeto.

*   **Definición:** Una secuencia finita de símbolos del alfabeto.
*   **Ejemplo 1:** "10110" (cadena binaria)
*   **Ejemplo 2:** "hola" (cadena de letras)
*   **Ejemplo 3:** "🔴 🟡 🟢" (cadena de colores de semáforo)

---

##### Lenguaje (L): El Diccionario Aprobado ✅

> Un lenguaje es un conjunto de cadenas válidas.

*   **Definición:** Un conjunto de cadenas formadas a partir de un alfabeto.
*   **Ejemplo 1:** El lenguaje de todas las cadenas binarias que empiezan con "1": L = {1, 10, 11, 100, 101, ...}
*   **Ejemplo 2:** El lenguaje de todas las palabras en español 🇪🇸.

---

##### Estados, Transiciones, Estado Inicial y Estado de Aceptación: Las Reglas del Juego 🎲

*   **Estado:** Una "situación" en la que se encuentra el autómata 📍.
*   **Transición:** Cómo el autómata cambia de un estado a otro al leer un símbolo de entrada ➡️.
*   **Estado Inicial:** El estado donde el autómata comienza 🏁.
*   **Estado de Aceptación:** Un estado que indica que la cadena de entrada es válida (pertenece al lenguaje) 🏆.

---

##### Ejercicio Práctico (¡Crea tu Propio Lenguaje! 💡):

Define un alfabeto y crea un lenguaje de al menos 5 cadenas diferentes. Describe las reglas que definen tu lenguaje.


##### Caso Práctico (El Validador de Contraseñas 🛡️):

Imagina que quieres validar contraseñas que deben tener al menos 8 caracteres y contener al menos un número. ¿Cómo definirías el alfabeto y el lenguaje para este problema?

===

#### 3. Autómatas Finitos Deterministas (AFD) 🤖🔍

##### Definición Formal (¡No te Asustes! 🤯):

> Un AFD es un modelo matemático 📐 con 5 componentes: (Q, Σ, δ, q0, F)

*   **Q:** Un conjunto finito de estados 📍.
*   **Σ:** Un alfabeto finito 🔤.
*   **δ:** Una función de transición (que dice cómo cambiar de estado al leer un símbolo): δ(estado, símbolo) = nuevo_estado ➡️.
*   **q0:** El estado inicial (un estado de Q) 🏁.
*   **F:** Un conjunto de estados de aceptación (un subconjunto de Q) 🏆.

---

##### Ejemplos (¡Haciendo Conexiones! 🔗):

*   **Ejemplo 1: El Interruptor de Luz 💡:** Un autómata con dos estados (encendido 🔆, apagado 🌑) y una entrada ("pulsar").

*   **Ejemplo 2: Paridad de 1s:** Un autómata que acepta cadenas binarias con un número par de "1"s (ya lo vimos antes 😉).

---

##### Construcción de AFDs (¡Manos a la Obra! 🛠️):

**Ejemplo: Construye un AFD que acepte cadenas binarias que terminen con "01".**

1.  **Identifica los estados:** Necesitas recordar las últimas dos entradas. Entonces necesitas estados para:
    *   "No he visto nada relevante aún" (estado inicial)
    *   "Acabo de ver un 0"
    *   "Acabo de ver un 01" (estado de aceptación)
    *   "Acabo de ver un 1"
2.  **Dibuja el diagrama de estados ✏️:** Dibuja los estados como círculos ⚪ y las transiciones como flechas ➡️.
3.  **Define la función de transición:** Para cada estado y cada símbolo de entrada (0 o 1), dibuja una flecha al siguiente estado correcto.
4.  **Define el estado inicial y los estados de aceptación:** Marca el estado inicial 🏁 y los estados de aceptación (en este caso, solo el estado "Acabo de ver un 01") 🏆.

---

##### Ejercicio Práctico (¡Construye tu Propio AFD! 🏗️):

Diseña un AFD que acepte cadenas que contengan la subcadena "ab". Dibuja el diagrama de estados.

##### Caso Práctico (El Validador de Números de Teléfono 📱):

Simplificando mucho, imagina que quieres validar números de teléfono que deben empezar con "555". ¿Cómo diseñarías un AFD para esto? (Solo el diagrama de estados simplificado, no te preocupes por todos los detalles de los números de teléfono reales).

===

#### 4. Autómatas Finitos No Deterministas (AFN) 🤯🤔

##### Definición Formal (¡Casi Igual que un AFD! 🤓):

> Un AFN es muy parecido a un AFD, pero con una diferencia clave: ¡puede tener múltiples opciones para el siguiente estado! 😲

*   **Q:** Un conjunto finito de estados 📍.
*   **Σ:** Un alfabeto finito 🔤.
*   **δ:** Una función de transición que puede dar *un conjunto* de estados: δ(estado, símbolo) = {nuevo_estado1, nuevo_estado2, ...} ➡️.
*   **q0:** El estado inicial (un estado de Q) 🏁.
*   **F:** Un conjunto de estados de aceptación (un subconjunto de Q) 🏆.

---

##### Ejemplos (¡La Aventura de Elegir! 🧭):

*   En un AFN, al leer un símbolo, puedes "adivinar" 🤔 cuál es el camino correcto. Si *algún* camino te lleva a un estado de aceptación 🏆, la cadena es aceptada ✅.

##### Conversión de AFN a AFD (¡Haciendo Trampa! 🤫):

> Todo AFN puede convertirse a un AFD equivalente. Esto significa que puedes "simular" el no determinismo con un autómata determinista. 🤯

---

*   **Idea Principal:** Cada estado del AFD representa un *conjunto* de estados del AFN 📦.
*   **Algoritmo:** (Simplificado)
    1.  Comienza con el estado inicial del AFD, que es el conjunto que contiene solo el estado inicial del AFN.
    2.  Para cada estado del AFD y cada símbolo del alfabeto, calcula a qué conjunto de estados del AFN puedes llegar. Ese conjunto se convierte en un nuevo estado del AFD.
    3.  Repite el paso 2 hasta que no puedas crear nuevos estados en el AFD.
    4.  Los estados de aceptación del AFD son aquellos que contienen *al menos un* estado de aceptación del AFN 🏆.

---

##### Ejercicio Práctico (¡Convierte un AFN a AFD! 🔄):

Dibuja un AFN que acepte cadenas que contengan "ab" (igual que el ejercicio del AFD). Luego, intenta convertirlo a un AFD.

##### Caso Práctico (Búsqueda de Patrones con Flexibilidad 🤸):

Los AFNs son útiles para buscar patrones con cierta flexibilidad. Por ejemplo, buscar palabras que contengan "color" o "colour". ¿Cómo diseñarías un AFN para esto?

===

#### 5. Aplicaciones de los Autómatas 🚀

##### Compiladores (¡Traductores de Lenguaje! 🌐):

*   **Función:** Los compiladores traducen el código que escribes (en Python 🐍, Java ☕, etc.) a instrucciones que la computadora puede entender 💻.
*   **Cómo se usan los Autómatas:**
    *   **Análisis Léxico:** Un autómata divide tu código en "tokens" (palabras clave, operadores, variables, etc.) ✂️.
    *   **Análisis Sintáctico:** Otro autómata verifica que los tokens estén en el orden correcto (que la sintaxis de tu código sea correcta) ✅.

---

##### Búsqueda de Patrones (¡Encontrar la Aguja en el Pajar! 🔎):

*   **Función:** Encontrar una subcadena específica dentro de un texto más grande 📝.
*   **Cómo se usan los Autómatas:** Puedes construir un autómata que acepte solo las cadenas que contienen el patrón que buscas. Luego, puedes usar ese autómata para buscar el patrón en el texto.

---

##### Validación de Datos (¡Asegurando la Calidad! 🛡️):

*   **Función:** Verificar que los datos que ingresa un usuario cumplen con un formato específico (emails 📧, números de teléfono 📱, códigos postales ✉️, etc.).
*   **Cómo se usan los Autómatas:** Puedes construir un autómata que acepte solo las cadenas que cumplen con el formato deseado.

---

##### Ejercicio Práctico (¡Piensa en Aplicaciones! 🤔):

¿En qué otras situaciones crees que se podrían usar los autómatas? Da al menos tres ejemplos.

##### Caso Práctico (El Filtro de Spam 🗑️):

Imagina que quieres crear un filtro de spam que detecte correos electrónicos que contengan ciertas palabras clave (como "viagra" o "oferta"). ¿Cómo podrías usar los autómatas para esto? (Describe la idea general, no necesitas diseñar el autómata completo).

===

#### 6. Ejercicios Resueltos de Autómatas. 📝

---

##### Ejercicio 1: AFD para Cadenas con un Número Impar de 'a's

Diseña un Autómata Finito Determinista (AFD) que acepte cadenas sobre el alfabeto Σ = {a, b} que contengan un número impar de 'a's.

---

**Solución Explicada**

1.  **Estados:** Necesitamos dos estados:
    *   q0: Representa haber visto un número par de 'a's (estado inicial).
    *   q1: Representa haber visto un número impar de 'a's (estado de aceptación).
2.  **Transiciones:**
    *   Si estamos en q0 y leemos una 'a', pasamos a q1.
    *   Si estamos en q0 y leemos una 'b', permanecemos en q0.
    *   Si estamos en q1 y leemos una 'a', pasamos a q0.
    *   Si estamos en q1 y leemos una 'b', permanecemos en q1.

---

3.  **Diagrama de Estados:**

![alt text](0_Introduccion/image.png)


*   **Explicación:** El autómata comienza en q0 (par). Cada vez que ve una 'a', cambia de estado. Si termina en q1 al final de la cadena, significa que ha visto un número impar de 'a's, y la cadena es aceptada.

===

##### Ejercicio 2: AFN para Cadenas que Contienen la Subcadena "aba"

Diseña un Autómata Finito No Determinista (AFN) que acepte cadenas sobre el alfabeto Σ = {a, b} que contengan la subcadena "aba".

---

**Solución Explicada**

1.  **Estados:**
    *   q0: Estado inicial (no hemos visto nada relevante aún).
    *   q1: Hemos visto una 'a'.
    *   q2: Hemos visto "ab".
    *   q3: Hemos visto "aba" (estado de aceptación).
2.  **Transiciones:**
    *   Desde q0, con 'a', vamos a q1.  También podemos permanecer en q0 con 'a' o 'b' (para ignorar símbolos al principio).
    *   Desde q1, con 'b', vamos a q2.
    *   Desde q2, con 'a', vamos a q3.
    *   Desde q3, podemos permanecer en q3 con 'a' o 'b' (para aceptar cualquier cosa después de "aba").

---

3.  **Diagrama de Estados:**

![alt text](0_Introduccion/image-1.png)

*   **Explicación:** El autómata "busca" la secuencia "aba". Una vez que la encuentra, pasa al estado de aceptación y permanece allí, aceptando cualquier cadena que contenga "aba".

===

##### Ejercicio 3: Expresión Regular para Cadenas que Empiezan con 'a' y Terminan con 'b'

Escribe una expresión regular que describa el lenguaje de todas las cadenas sobre el alfabeto Σ = {a, b} que comienzan con 'a' y terminan con 'b'.

---

**Solución Explicada**

La expresión regular es: `a(a|b)*b`

*   **a:** La cadena debe comenzar con 'a'.
*   `(a|b)*`:  Después de la 'a' inicial, puede haber cualquier número (cero o más) de 'a's o 'b's.  `(a|b)` significa "a o b", y `*` significa "cero o más repeticiones".
*   **b:** La cadena debe terminar con 'b'.

**Ejemplos de cadenas aceptadas:**

*   ab
*   aab
*   abb
*   aaabb
*   ababab

===

##### Ejercicio 4: Convertir un AFN a AFD (Simplificado)

Dado el siguiente AFN, conviértelo a un AFD equivalente:

*   Estados: {q0, q1}
*   Alfabeto: {0, 1}
*   Estado Inicial: q0
*   Estado de Aceptación: q1
*   Transiciones:
    *   δ(q0, 0) = {q0, q1}
    *   δ(q0, 1) = {q0}
    *   δ(q1, 0) = {} (conjunto vacío)
    *   δ(q1, 1) = {q1}

---

**Solución Explicada**

1.  **Estado Inicial del AFD:** {q0}
2.  **Transiciones desde {q0}:**
    *   Con 0: δ({q0}, 0) = {q0, q1} (nuevo estado del AFD)
    *   Con 1: δ({q0}, 1) = {q0} (estado ya existente)
3.  **Transiciones desde {q0, q1}:**
    *   Con 0: δ({q0, q1}, 0) = δ(q0, 0) ∪ δ(q1, 0) = {q0, q1} ∪ {} = {q0, q1} (estado ya existente)
    *   Con 1: δ({q0, q1}, 1) = δ(q0, 1) ∪ δ(q1, 1) = {q0} ∪ {q1} = {q0, q1} (estado ya existente)

---

4.  **Estados de Aceptación del AFD:** {q0, q1} (porque contiene q1, que es un estado de aceptación del AFN)

**AFD Resultante:**

*   Estados: { {q0}, {q0, q1} }
*   Alfabeto: {0, 1}
*   Estado Inicial: {q0}
*   Estado de Aceptación: {{q0, q1}}
*   Transiciones:
    *   δ({q0}, 0) = {q0, q1}
    *   δ({q0}, 1) = {q0}
    *   δ({q0, q1}, 0) = {q0, q1}
    *   δ({q0, q1}, 1) = {q0, q1}

===

##### Ejercicio 5:  Lenguaje Aceptado por un AFD Dado

Describe en palabras el lenguaje aceptado por el siguiente AFD:

*   Estados: {q0, q1, q2}
*   Alfabeto: {a, b}
*   Estado Inicial: q0
*   Estado de Aceptación: {q2}
*   Transiciones:
    *   δ(q0, a) = q1
    *   δ(q0, b) = q0
    *   δ(q1, a) = q1
    *   δ(q1, b) = q2
    *   δ(q2, a) = q1
    *   δ(q2, b) = q2

---

**Solución Explicada**

El AFD acepta todas las cadenas que contienen al menos una 'a' seguida inmediatamente por una 'b'.

*   **Explicación:**
    *   Desde el estado inicial q0, el autómata permanece en q0 si lee una 'b'.
    *   Si lee una 'a', pasa al estado q1.
    *   Desde q1, si lee una 'b', pasa al estado de aceptación q2.
    *   Una vez en q2, el autómata permanece en q2 sin importar si lee 'a' o 'b'.

**Ejemplos de cadenas aceptadas:**

*   ab
*   aab
*   bab
*   bbab
*   aaabbb

---

**Ejemplos de cadenas rechazadas:**

*   a
*   b
*   bb
*   aaa