Palabra Clave/Término	Definición	Ejemplo
await	Se usa en funciones asíncronas para pausar la ejecución hasta que se complete una operación async.	datos = await obtener_datos()
async	Se usa para declarar una función como corutina, permitiendo que se ejecute de forma asíncrona.	async def tarea(): await asyncio.sleep(1)
yield from	Se usa dentro de un generador para delegar parte de la operación a otro generador o iterador.	yield from otra_funcion_generadora()
property	Decorador que convierte un método de clase en una propiedad (atributo) de solo lectura o con setters.	@property
setter	Método para establecer o modificar el valor de una propiedad, usado junto con @property.	@nombre.setter
getter	Método para obtener o leer el valor de una propiedad, definido con @property.	valor = mi_objeto.propiedad
decorator	Una función que envuelve a otra función para modificar su comportamiento sin cambiar su código.	@mi_decorador
dict	Abreviatura para diccionario, una colección desordenada de pares clave-valor.	mi_dict = {"clave": 1}
list	Tipo de dato que representa una colección ordenada y mutable de elementos.	mi_lista = [1, 2, 3]
tuple	Tipo de dato que representa una colección ordenada e inmutable de elementos.	mi_tupla = (1, 2)
set	Tipo de dato para una colección no ordenada de elementos únicos.	mi_set = {1, 2, 3}
f-string	Una cadena literal prefijada con 'f', que permite la interpolación (incrustar expresiones).	f"El valor es {x}"
slice	Una forma de seleccionar un subconjunto de elementos de una secuencia (lista, tupla, cadena) usando [inicio:fin:paso].	mi_lista[1:4]
comprehension	Una sintaxis concisa para crear listas, diccionarios o conjuntos (ej. list comprehension).	[i*2 for i in range(5)]
iterable	Un objeto que puede ser recorrido (iterado) elemento por elemento, como listas, tuplas, etc.	for item in mi_iterable:
iterator	Un objeto que implementa los métodos __iter__ y __next__ para seguir la pista de la iteración.	it = iter(mi_lista); next(it)
context manager	Un objeto que define los métodos __enter__ y __exit__, usado con la instrucción with.	with open(...) as f:
docstring	Una cadena literal usada para documentar módulos, clases, funciones o métodos.	def fn(): """Documentación aquí"""
__init__	El constructor de una clase, llamado al crear una nueva instancia (objeto).	def __init__(self): ...
__str__	Método que devuelve una representación legible de un objeto, usado por print().	def __str__(self): return "..."
__repr__	Método que devuelve una representación formal del objeto, usada a menudo para depuración.	def __repr__(self): return "..."
classmethod	Decorador que indica que un método está vinculado a la clase y no a la instancia.	@classmethod
staticmethod	Decorador que indica que un método no depende ni de la clase ni de la instancia.	@staticmethod
self	Convención para el primer parámetro de un método de instancia, refiriéndose a la propia instancia (objeto).	def metodo(self): ...
args	Convención para un número variable de argumentos posicionales en una función, representado por *args.	def fn(*args):
kwargs	Convención para un número variable de argumentos de palabra clave en una función, representado por **kwargs.	def fn(**kwargs):
pass	Ya incluido.	(No se añade)
assert	Ya incluido.	(No se añade)
isinstance	Función para verificar si un objeto es una instancia de una clase o un tipo de datos.	isinstance(x, list)
issubclass	Función para verificar si una clase hereda de otra.	issubclass(Perro, Animal)
super	Se refiere a la clase padre o superclase de la clase actual, a menudo usado en __init__.	super().__init__()
mro	Abreviatura para Method Resolution Order (Orden de Resolución de Métodos), el orden en que Python busca métodos en jerarquías de herencia.	Clase.mro()
pip	Acrónimo de "Pip Installs Packages", el sistema de gestión de paquetes estándar para Python.	pip install requests
venv	Abreviatura de "Virtual Environment", un entorno aislado para proyectos de Python.	python -m venv mi_venv
path	Se refiere a la ubicación de un archivo o directorio en el sistema de archivos.	os.path.join(...)
os	Módulo que proporciona una forma de interactuar con el sistema operativo.	import os
sys	Módulo que proporciona acceso a variables y funciones que interactúan con el intérprete de Python.	import sys; sys.exit()
pdb	El debugger interactivo de Python.	import pdb; pdb.set_trace()
gil	Acrónimo de "Global Interpreter Lock", un mecanismo que asegura que solo un hilo de Python se ejecute a la vez.	(Concepto de concurrencia)
id()	Función que devuelve la identidad única de un objeto (su dirección en memoria).	id(x) == id(y)
hash()	Función que devuelve el valor hash de un objeto, usado para claves de diccionario.	hash(mi_tupla)
immutable	Se refiere a un objeto (como una tupla o cadena) cuyo valor no puede ser cambiado después de su creación.	mi_tupla[0] = 5 (Error)
mutable	Se refiere a un objeto (como una lista o diccionario) cuyo valor puede ser cambiado después de su creación.	mi_lista[0] = 5 (Válido)
zip()	Función que combina múltiples iterables, elemento por elemento, en una tupla de tuplas.	list(zip(a, b))
map()	Función que aplica una función a cada elemento de un iterable y devuelve un nuevo iterable.	list(map(str, nums))
filter()	Función que filtra elementos de un iterable basándose en una función que devuelve True o False.	list(filter(es_par, nums))
globals()	Función que devuelve un diccionario que contiene las variables del ámbito global.	print(globals()['variable_global'])
locals()	Función que devuelve un diccionario que contiene las variables del ámbito local actual.	print(locals()['variable_local'])
eval()	Función que ejecuta dinámicamente una cadena como código de Python.	eval("1 + 1")
exec()	Función que ejecuta dinámicamente un bloque de código Python (como una cadena o un objeto de código).	exec("x = 10; print(x)")
try	Ya incluido.	(No se añade)
except	Ya incluido.	(No se añade)
finally	Se utiliza en el manejo de excepciones para el código que siempre se ejecutará, haya o no error.	try: ... except: ... finally: print("Siempre se ejecuta")
