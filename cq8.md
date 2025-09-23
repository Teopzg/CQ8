1. KeyError
¿Qué lo causa? Se produce cuando intentas acceder a una clave que no existe en un diccionario.

Ejemplo:

Python

mi_dict = {"a": 1, "b": 2}
print(mi_dict["c"])
Cómo corregirlo: Asegúrate de que la clave exista antes de acceder a ella, utilizando if key in dict o el método .get() para proporcionar un valor predeterminado.

2. IndexError
¿Qué lo causa? Ocurre cuando intentas acceder a un índice que está fuera del rango de una lista, tupla o cadena.

Ejemplo:

Python

mi_lista = [10, 20]
print(mi_lista[2])
Cómo corregirlo: Verifica que el índice que estás utilizando sea válido. Recuerda que los índices comienzan en 0 y terminan en len(lista) - 1.

3. TypeError
¿Qué lo causa? Se produce cuando una operación o función se aplica a un objeto de un tipo inapropiado, como intentar sumar un número a una cadena.

Ejemplo:

Python

cadena = "Hola"
numero = 5
print(cadena + numero)
Cómo corregirlo: Asegúrate de que las variables que estás operando sean del tipo de dato correcto. Si es necesario, usa funciones como str(), int() o float() para convertir los tipos.

4. NameError
¿Qué lo causa? Se lanza cuando intentas usar una variable, función o módulo que no ha sido definido o declarado.

Ejemplo:

Python

print(mi_variable)
Cómo corregirlo: Define la variable antes de usarla, o verifica que el nombre de la variable o función esté bien escrito.

5. IndentationError
¿Qué lo causa? Es un error de sintaxis que ocurre cuando hay un problema con la indentación del código, como un espacio extra o una tabulación incorrecta.

Ejemplo:

Python

if True:
  print("Hola")
Cómo corregirlo: Python usa la indentación para definir bloques de código. Asegúrate de que cada línea esté correctamente indentada con 4 espacios (o una tabulación).

6. ZeroDivisionError
¿Qué lo causa? Ocurre cuando intentas dividir un número por cero, lo cual es una operación matemática indefinida.

Ejemplo:

Python

resultado = 10 / 0
Cómo corregirlo: Agrega una condición que verifique si el divisor es cero antes de realizar la división, o usa un bloque try-except para manejar la excepción.

7. ValueError
¿Qué lo causa? Se produce cuando una función recibe un argumento del tipo de dato correcto, pero con un valor inapropiado (por ejemplo, cuando intentas convertir una cadena que no es un número a un entero).

Ejemplo:

Python

numero = int("abc")
Cómo corregirlo: Valida el valor de la entrada del usuario o usa un bloque try-except para capturar este error y manejarlo de forma elegante.

8. AttributeError
¿Qué lo causa? Ocurre cuando intentas acceder a un atributo o método que no existe para un tipo de objeto específico.

Ejemplo:

Python

lista = [1, 2, 3]
lista.uppercase()
Cómo corregirlo: Verifica que el objeto tenga el atributo o método que intentas usar. A menudo, esto sucede por una simple falta de ortografía en el nombre del método.

9. SyntaxError
¿Qué lo causa? Es un error de sintaxis que ocurre cuando el código no sigue las reglas gramaticales del lenguaje.

Ejemplo:

Python

if x > 5
  print("x es mayor que 5")
Cómo corregirlo: Revisa la sintaxis de tu código. En este caso, faltan los dos puntos (:) después de la condición if.

10. ImportError
¿Qué lo causa? Se produce cuando intentas importar un módulo que no se encuentra o que no puede ser cargado.

Ejemplo:

Python

import mi_modulo_inexistente
Cómo corregirlo: Asegúrate de que el módulo esté instalado y que el nombre del módulo esté bien escrito.

11. FileNotFoundError
¿Qué lo causa? Ocurre cuando intentas acceder a un archivo que no existe en la ruta especificada.

Ejemplo:

Python

with open("archivo_que_no_existe.txt", "r") as f:
  contenido = f.read()
Cómo corregirlo: Verifica que la ruta y el nombre del archivo sean correctos.

12. MemoryError
¿Qué lo causa? Se produce cuando el programa se queda sin memoria para continuar su ejecución, generalmente por crear objetos demasiado grandes o estructuras de datos ineficientes.

Ejemplo:

Python

lista_enorme = [i for i in range(10**9)]
Cómo corregirlo: Optimiza tu código para usar menos memoria. Considera usar generadores o procesar los datos en fragmentos más pequeños.

13. RecursionError
¿Qué lo causa? Ocurre cuando una función recursiva se llama a sí misma demasiadas veces sin una condición de parada, excediendo el límite de recursión.

Ejemplo:

Python

def funcion_infinita():
  funcion_infinita()
funcion_infinita()
Cómo corregirlo: Asegúrate de que tu función recursiva tenga una condición de parada clara y accesible.

14. StopIteration
¿Qué lo causa? Se lanza por la función next() de un iterador cuando no hay más elementos para iterar.

Ejemplo:

Python

mi_iterador = iter([1, 2])
next(mi_iterador)
next(mi_iterador)
next(mi_iterador)
Cómo corregirlo: Usa un bucle for para iterar, que maneja automáticamente esta excepción, o maneja el error con un bloque try-except si usas next() directamente.
