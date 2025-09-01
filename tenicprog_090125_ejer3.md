# Problema 3: Acceso a un parque de diversiones

Queremos que un programa decida si una persona puede acceder a un parque de 
diversiones y a qué atracciones puede subir.  

**Requisitos:**
- La persona debe ser mayor de 12 años para poder ingresar al parque.  
- Dentro del parque, si mide más de 1,60 metros, puede subir a la montaña rusa.  
- Si no cumple con la altura, solo podrá acceder a los juegos infantiles.  
- Si es menor de 12 años, no puede ingresar al parque.  
- Investigar qué son los condicionales anidados en Python y cómo funcionan.  
- Documentar todo el proceso de resolución.  
- Guardar y mostrar la conversación con IA si se utilizó.  
- Explicar debates o decisiones tomadas durante la resolución.  
- Documentar paso a paso la construcción de la solución.  
- Explicar qué hace cada línea de código y justificar su uso.  
- Asegurarse de explicar los conceptos básicos: condicionales, operadores de comparación y anidación de estructuras.  

## Solución en Python

```python
# Un diccionario donde cada clave es el nombre de la persona (str)
# y el valor es una tupla con su edad y altura (int, float)
personas = {
    "Ana": (15, 1.70),
    "Carlos": (10, 1.50),
    "Lucía": (18, 1.65),
    "Pedro": (20, 1.55),
    "Sofía": (12, 1.40)
}

# Bucle 'for' para recorrer el diccionario
# El método .items() nos permite acceder a la clave (nombre) y al valor (datos de la persona)
for nombre, datos in personas.items():
    # Desempaquetar la tupla de datos para acceder a la edad y la altura
    edad = datos[0]
    altura = datos[1]

    # Imprimir los datos de la persona actual para un mejor seguimiento
    print(f"\nProcesando a {nombre} de {edad} años y {altura} metros:")

    # Lógica condicional anidada para el acceso al parque y atracciones
    if edad >= 12:
        print("  ¡Puede ingresar al parque!")
        if altura > 1.60:
            print("  ¡Puede subir a la montaña rusa!")
        else:
            print("  Solo puede acceder a los juegos infantiles.")
    else:
        print("  No puede ingresar al parque.")

