Conversación ChatGPT : https://chatgpt.com/share/68b62526-b35c-8005-a312-5cf36e24c018

1) Introducción — ¿qué es una variable y tipos básicos en Python?
Una variable es un nombre que apunta a un valor almacenado en memoria. En Python las variables son dinámicamente tipadas: no declares el tipo al crearla, el intérprete lo infiere por el valor asignado.
Tipos básicos importantes:

str — cadena de texto (p. ej. "Hola").
int — enteros (p. ej. 42).
float — números con decimales (usa punto: 1.75).
bool — booleano: True o False.
list — lista ordenada y mutable: colección de valores [a, b, c].

2) Proceso y decisiones

Decisiones tomadas para cada variable del enunciado:
nombre → str: representa texto (nombre propio).
edad → int: número entero sin decimales.
altura → float: altura requiere decimales; usar punto (1.75), no coma.
es_estudiante → bool: verdadero/falso para estado.
materias → list: varias materias en orden, posibilidad de modificar (agregar/quitar).

Errores comunes:
Escribir 1,75 — en Python eso crea una tupla (1, 75) o provocará comportamiento inesperado; use 1.75.
Usar nombres de variables que empiezan con número o con espacios: inválido (1edad no OK).
Usar palabras reservadas (class, def, if) como nombre de variable.
Confundir comillas simples y dobles no es crítico ('a' = "a"), pero mantener consistencia.

Convenciones:
snake_case para nombres: es_estudiante, lista_materias.
Si el valor puede ser desconocido inicialmente, usar None (tipo NoneType) y documentarlo.

3) Código en Python (minimal y correcto), con comentarios línea por línea

# Datos del alumno: declaración de variables con tipos básicos

nombre = "Francisco Ramasco"   # str: nombre completo como texto
edad = 35                      # int: edad como número entero
altura = 1.75                  # float: altura en metros; usar punto decimal
es_estudiante = True           # bool: True si es estudiante, False en caso contrario
materias = ["Programación I", "Matemática", "Redes"]  # list: lista ordenada de materias

# Comprobación opcional (muestra tipo y valor) - útil para depurar
print(type(nombre), nombre)
print(type(edad), edad)
print(type(altura), altura)
print(type(es_estudiante), es_estudiante)
print(type(materias), materias)


4) Explicación de tipos con ejemplos adicionales (y por qué son útiles)

str (cadena)
Ejemplo: saludo = "Hola, " + nombre
Uso: representar texto, concatenarlo, formatearlo. Utile para mostrar mensajes al usuario.
int (entero)
Ejemplo: años_para_100 = 100 - edad
Uso: contar, índices, operaciones aritméticas sin decimales.
float (decimal)
Ejemplo: altura_mas_ajuste = altura + 0.05
Uso: medidas, promedios, cálculos que requieren fracciones. Usar punto para decimales.
bool (booleano)
Ejemplo:

if es_estudiante:
    print("Está cursando la tecnicatura")
else:
    print("No es estudiante")
# Uso: decisiones, condiciones, filtros.


list (lista)
Ejemplo:

primera_materia = materias[0]     # acceso por índice (0 es el primero)
materias.append("Algoritmos")     # agregar una materia al final
# Uso: colecciones ordenadas y mutables — ideal para conjuntos de materias, notas, etc.

5) Paso a paso seguido (documentación del proceso)

Leer el enunciado y mapear cada dato a un tipo lógico (texto, número entero, número decimal, booleano, colección).
Elegir nombres de variables descriptivos y en snake_case.
Elegir valores ejemplo realistas (edad como entero, altura con punto decimal).
Escribir declaraciones mínimas en Python.
Añadir comentarios explicativos por línea (documentación).
Probar con print() y type() para verificar tipos.
Documentar decisiones y errores comunes (puntos 2 y 6).

6) Debate / decisiones y alternativas consideradas

Alternativas y por qué no las elegí por ahora:
tuple en vez de list para materias: si las materias no se van a modificar, tuple (("Prog", "Mat")) ofrece inmutabilidad. Elegí list porque suele ser práctico agregar/quitar materias en ejercicios iniciales.
Usar None como valor inicial si no se conoce la información: p. ej. altura = None. Esto requiere comprobaciones antes de usarlo. No lo usé porque el enunciado pide declarar valores concretos.
Type hints: nombre: str = "..." (opcional). Es útil para documentación y herramientas (linters/IDE), pero no es obligatorio en Python.
Estructura más compleja: usar dict o dataclass para agrupar todos los atributos del alumno:

alumno = {"nombre": "...", "edad": 35, "altura": 1.75, "es_estudiante": True, "materias": [...]}
# Esto es útil cuando manejas muchos alumnos, pero la consigna pide declarar variables sueltas para aprender tipos básicos.

Decisiones prácticas:
Mantener el ejemplo simple para centrarse en la comprensión de tipos.
Documentar el uso de punto decimal y problemas comunes.

7) Conclusiones / aprendizajes

Las variables son etiquetas para valores; Python infiere su tipo.
Conocer y elegir el tipo correcto evita errores y facilita operaciones posteriores.
Errores típicos iniciales: usar coma en lugar de punto para floats, nombres inválidos, y confundir mutabilidad.
Practicar con type() y operaciones sencillas (concatenación, operaciones aritméticas, append en listas) ayuda a consolidar conceptos.
