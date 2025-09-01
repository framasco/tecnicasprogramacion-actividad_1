# Problema 2: Control de entrada al cine

Queremos que un programa nos diga si una persona puede entrar a un cine.  
La condición es que **solo pueden entrar los mayores de 18 años**.  
Si la persona tiene 18 años o más, el programa debe mostrar un mensaje indicando que puede entrar; de lo contrario, debe mostrar que no puede entrar.  

---

## Objetivos de la actividad
- Investigar qué es una **estructura condicional (`if / else`)** en Python y cómo funciona.  
- Documentar todo el proceso de resolución.  
- Si se utilizó una IA como apoyo, guardar y mostrar la conversación completa.  
- Explicar qué debates o decisiones se tomaron para resolver el problema.  
- Documentar el paso a paso seguido para construir la solución.  
- Explicar qué hace cada línea del código y justificar por qué se escribió de esa forma.  
- Explicar los conceptos básicos que aparecen en el código: **variables, operadores de comparación, condicionales**.

---

## Proceso y decisiones

Para este ejercicio se decidió:
- Guardar la información de cada persona en un **diccionario**, que contiene `nombre` y `edad`.  
- Agrupar todos los diccionarios en una **lista**, para poder recorrerla fácilmente.  
- Usar un **bucle `for`** para recorrer cada persona de la lista.  
- Evaluar con un **`if / else`** si cada persona puede entrar según su edad.  

Esta estructura permite agregar más personas o atributos en el futuro de manera sencilla.

---

## Código en Python

```python
# Lista de personas, cada una representada como un diccionario
personas = [
    {"nombre": "Francisco", "edad": 35},
    {"nombre": "Micaela", "edad": 25},
    {"nombre": "Valentin", "edad": 17}
]

# Recorremos cada persona en la lista
for persona in personas:
    # Condicional: verificamos si la persona tiene 18 años o más
    if persona["edad"] >= 18:
        print(f"{persona['nombre']} puede entrar al cine.")  # Mensaje si cumple la condición
    else:
        print(f"{persona['nombre']} no puede entrar al cine.")  # Mensaje si no cumple


