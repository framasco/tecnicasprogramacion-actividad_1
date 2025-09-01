Tarea de Técnicas de Programación
1. Introducción: Variables y tipos de datos en Python
Una variable es un nombre que apunta a un valor almacenado en la memoria. En Python, las variables son de tipado dinámico, lo que significa que no necesitas declarar su tipo; el intérprete lo infiere automáticamente al asignar un valor.

Los tipos de datos básicos que utilizaremos son:

str (string): Para texto (ej. "Hola Mundo").

int (integer): Para números enteros (ej. 42).

float: Para números con decimales (siempre usando un punto, ej. 1.75).

bool (boolean): Para valores de verdad (True o False).

list: Para colecciones ordenadas y mutables de valores (ej. ["a", "b"]).

2. Proceso y decisiones
Elección de tipos de datos
Para cada variable solicitada, se eligió el tipo de dato más adecuado:

nombre → str: Representa texto.

edad → int: Número entero sin decimales.

altura → float: Requiere decimales.

es_estudiante → bool: Representa un estado binario (verdadero/falso).

materias → list: Es una colección de elementos que puede cambiar (se pueden agregar o quitar materias).

Errores comunes y convenciones
Separador de decimales: Se usó el punto (.) en la variable altura. Un error común es usar la coma (,), lo que Python interpreta como una tupla, no como un número decimal.

Nombres de variables: Se usó la convención snake_case (es_estudiante) para mejorar la legibilidad del código y se evitaron nombres que empiecen con números o usen palabras reservadas de Python.

3. Código en Python
A continuación, se presenta el código minimalista y correcto, con comentarios explicativos.

# 1. Declaración de variables con tipos básicos.

nombre = "Francisco Ramasco"    # str: Almacena el nombre completo.
edad = 35                      # int: Almacena la edad como un número entero.
altura = 1.75                  # float: Almacena la altura usando punto decimal.
es_estudiante = True           # bool: Indica si la persona es estudiante (True) o no (False).
materias = ["Programación I", "Matemática", "Redes"]  # list: Colección de las materias que cursa.

# 2. Comprobación opcional del tipo y valor de las variables.
print(f"Tipo: {type(nombre)} -> Valor: {nombre}")
print(f"Tipo: {type(edad)} -> Valor: {edad}")
print(f"Tipo: {type(altura)} -> Valor: {altura}")
print(f"Tipo: {type(es_estudiante)} -> Valor: {es_estudiante}")
print(f"Tipo: {type(materias)} -> Valor: {materias}")

4. Explicación de tipos con ejemplos adicionales
str (string): útil para representar cualquier dato de texto, como mensajes o descripciones.

Ejemplo: saludo = "Hola, " + nombre

int (integer): útil para operaciones aritméticas sin decimales, como contadores o índices.

Ejemplo: años_restantes = 100 - edad

float: útil para medidas, promedios y cálculos que requieren precisión decimal.

Ejemplo: altura_nueva = altura + 0.05

bool (boolean): fundamental para la lógica de los programas, permitiendo tomar decisiones en base a condiciones.

Ejemplo:


if es_estudiante:
    print("Está cursando la tecnicatura")
list (lista): ideal para colecciones de datos ordenadas y mutables.

Ejemplo:


# Acceso a un elemento por su posición (índice 0)
primera_materia = materias[0]
# Agregar un elemento a la lista
materias.append("Algoritmos")

5. Paso a paso del proceso
Mapeo: Identifiqué cada dato de la consigna y lo asocié a un tipo de variable lógico.

Codificación: Escribí las declaraciones de las variables con valores realistas.

Documentación: Añadí comentarios en el código y explicaciones detalladas en el texto.

Verificación: Usé la función type() para confirmar que las variables almacenan los tipos de datos correctos.

6. Debate y alternativas
Se consideraron otras estructuras de datos como tuple (inmutable) o dict (diccionario) para agrupar los datos. Si bien un dict es útil para representar un único alumno con todos sus atributos, la consigna pedía declarar variables separadas para enfocarse en los tipos de datos básicos individualmente. Esto ayudó a mantener el ejemplo simple y pedagógico.

7. Conclusiones y aprendizajes
Esta actividad me permitió reafirmar que las variables son esenciales para almacenar información y que la elección del tipo de dato es crucial para el correcto funcionamiento del programa. Los errores comunes, como el uso de la coma en lugar del punto, resaltan la importancia de prestar atención a la sintaxis del lenguaje. El uso de nombres descriptivos y la documentación con comentarios son buenas prácticas que mejoran la calidad del código.

8. Transcripción del chat
(Enlace a la conversación de ChatGPT)

Esta conversación fue utilizada como punto de partida para generar la estructura inicial del documento, que luego fue revisada, ampliada y adaptada para cumplir con los requisitos específicos de la consigna.
