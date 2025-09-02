
# Problema 4: Simulación de una caminata

Queremos simular una caminata. La idea es que el programa muestre en pantalla cómo una 
persona va dando pasos, desde el paso 1 hasta el paso 10. Para lograrlo, necesitamos que 
el programa repita una acción varias veces sin escribir la misma instrucción muchas veces.  

**Requisitos:**
- Investigar qué es un bucle `while` en Python y cómo funciona.  
- Documentar todo el proceso de resolución.  
- Guardar y mostrar la conversación con IA si se utilizó.  
- Explicar debates o decisiones tomadas durante la resolución.  
- Documentar paso a paso la construcción de la solución.  
- Explicar qué hace cada línea de código y justificar su uso.  
- Asegurarse de explicar los conceptos básicos: variables, condiciones, incremento, etc.  

**Decisiones de diseño:**
- Se eligió un **bucle `while`** porque la consigna pide repetir una acción varias veces.  
- **Variable de control:** `paso`, inicializada en 1 para que el conteo comience desde el primer paso.  
- **Condición del bucle:** `while paso <= 10` asegura que se incluyan los 10 pasos y se detenga justo después.  
- **Actualización de la variable:** `paso += 1` incrementa la variable en cada iteración, evitando un bucle infinito.  

## Solución en Python

```python
# 1. Inicialización de la variable de control
# Creamos la variable 'paso' y le asignamos el valor inicial de 1.
paso = 1

# 2. Bucle 'while'
# El bucle se ejecutará MIENTRAS el valor de 'paso' sea menor o igual a 10.
while paso <= 10:
    # 3. Acción a repetir
    # Mostramos en pantalla el número del paso actual.
    print(f"Dando el paso número {paso}")
    
    # 4. Actualización de la variable de control
    # Incrementamos el valor de 'paso' en 1 para avanzar en el conteo.
    paso += 1
    
# 5. Salida del bucle
# Cuando la variable 'paso' sea 11, la condición se vuelve falsa y el bucle termina.
print("¡Caminata completada!")
