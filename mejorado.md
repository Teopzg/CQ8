| No. | Excepción/Error | Lenguaje(s) | Causa Principal | Corrección Sugerida |
| :---: | :--- | :--- | :--- | :--- |
| 1 | **KeyError** | Python | Acceso a una **clave** inexistente en un diccionario. | Usar `dict.get(key, default)` o verificar la existencia de la clave (`if key in dict:`). |
| 2 | **IndexError** | Python | Acceso a un **índice** fuera de los límites de una lista/tupla. | Asegurar que el índice esté entre `0` y `longitud - 1`. |
| 3 | **ZeroDivisionError** | Python | División o módulo por **cero**. | Usar `try-except` para manejar la operación o comprobar el divisor. |
| 4 | **NameError** | Python | Uso de una **variable** o función que no ha sido definida o está fuera de alcance. | Asegurar la declaración y accesibilidad de la variable en el ámbito. |
| 5 | **SyntaxError** | Python/Java | Romper las **reglas de gramática** (ej. olvidar `:` en Python, `;` en Java). | Revisar cuidadosamente la línea de código indicada por el intérprete/compilador. |
| 6 | **AttributeError** | Python | Intento de acceder a un **atributo** o método inexistente en un objeto. | Verificar la ortografía del atributo o revisar la documentación del objeto. |
| 7 | **TypeError** | Python | Aplicación de una operación a un objeto del **tipo incorrecto**. | Usar **conversión de tipos** explícita (`str()`, `int()`) o verificar el tipo. |
| 8 | **ValueError** | Python | Argumento con **valor inapropiado** (aunque el tipo sea correcto) para una función. | Validar la entrada del usuario o los parámetros de la función antes de la llamada. |
| 9 | **IOError/FileNotFoundError**| Python | Acceso a un **archivo** que no existe o el programa no tiene permisos. | Verificar la ruta del archivo o usar `try-except` para manejo de archivos. |
| 10 | **MemoryError** | Python | El intérprete se queda sin **memoria** (ej. recursión infinita o estructuras muy grandes). | Optimizar el código para usar menos memoria o reducir el tamaño de las estructuras. |
| 11 | **ImportError** | Python | Fallo al **importar** un módulo; no existe o hay un error circular de importación. | Verificar que el módulo esté instalado (`pip`) y las dependencias circulares. |
| 12 | **TabError** | Python | Indentación con **mezcla** inconsistente de tabulaciones y espacios. | Configurar el editor para usar consistentemente espacios (recomendado en Python). |
| 13 | **ArithmeticException** | Java | Operaciones aritméticas ilegales (división por cero con **enteros**). | Incluir una comprobación de división por cero antes de la operación. |
| 14 | **NullPointerException** | Java | Intento de usar una **referencia** de objeto que apunta a **null**. | Inicializar el objeto con `new` o verificar si es `null` antes de usarlo. |
| 15 | **ArrayIndexOutOfBoundsException** | Java | Acceso a un índice **fuera de los límites** de un array. | Usar `array.length` para verificar los límites en los accesos. |
| 16 | **ClassCastException** | Java | Intento de convertir un objeto a una **subclase** de la que no es realmente una instancia. | Usar `instanceof` para verificar el tipo antes de intentar la conversión. |
| 17 | **IllegalArgumentException** | Java | Llamada a un método con un **argumento ilegal o inapropiado**. | Validar el argumento del método o verificar el contrato del método. |
| 18 | **NumberFormatException** | Java | Intento de convertir una cadena (`String`) en un **tipo numérico** inválido. | Usar el manejo de excepciones o funciones de validación de cadenas. |
| 19 | **IOException** | Java | Error durante la operación de **entrada/salida** (lectura/escritura de archivos). | Usar `try-catch` y asegurar el cierre de recursos con `finally` o `try-with-resources`. |
| 20 | **NoSuchMethodException** | Java | Intento de acceder a un método usando **Reflection** que no existe. | Verificar la firma del método que se está buscando. |
| 21 | **SecurityException** | Java | Se ha violado una **restricción de seguridad**. | Ajustar la política de seguridad o la configuración del entorno. |
| 22 | **StackOverflowError** | Java | Ocurre una **recursión infinita** o excesivamente profunda, llenando la pila. | Revisar la condición base de la función recursiva para asegurar su terminación. |
| 23 | **ConcurrentModificationException** | Java | Una **colección** es modificada mientras es iterada por otro hilo o dentro del mismo iterador. | Usar colecciones concurrentes o iteradores explícitos. |
| 24 | **InterruptedException** | Java | Un **hilo** que está esperando, durmiendo o bloqueado, es interrumpido por otro hilo. | Manejar la excepción, a menudo restableciendo el estado de interrupción. |
| 25 | **IllegalStateException** | Java | Un método es llamado en un **momento inapropiado** o cuando el objeto no está en un estado válido. | Revisar el ciclo de vida del objeto y asegurar la secuencia correcta de llamadas. |
| 26 | **AssertionError** | Python/Java | Una **aserción** (`assert`) falla en una prueba condicional. | Indica un error lógico en el código que debe ser corregido antes de la ejecución. |
| 27 | **UnicodeDecodeError** | Python | Fallo al **decodificar** bytes a una cadena usando un *encoding* incorrecto. | Especificar el *encoding* correcto al abrir o leer el archivo. |
| 28 | **NotImplementedError** | Python | Un método que se esperaba **implementar** en una subclase no lo está. | Proporcionar la lógica del método en la subclase. |
| 29 | **RecursionError** | Python | Una función **recursiva** se llama a sí misma demasiadas veces (límite de profundidad). | Ajustar el límite de recursión o refactorizar a un enfoque iterativo. |
| 30 | **SystemExit** | Python | Excepción lanzada por `sys.exit()` que indica una **terminación** normal. | Generalmente se atrapa solo para limpieza o logging. |
| 31 | **UnknownHostException** | Java | Fallo de conexión a red cuando el nombre del servidor **no puede ser resuelto**. | Verificar la conexión a internet o el nombre del host (DNS). |
| 32 | **SocketTimeoutException** | Java | Una operación de red (socket) **excede** el tiempo de espera establecido. | Aumentar el tiempo de espera o verificar la disponibilidad del servidor. |
| 33 | **Unchecked Exception** | Java | Excepciones que heredan de `RuntimeException` (no se requiere `try/catch` explícito). | Corregir el error lógico del código que la causa (ej. `NullPointerException`). |
| 34 | **Checked Exception** | Java | Excepciones que **deben** ser manejadas con `try/catch` o declaradas con `throws`. | Añadir el bloque `try-catch` o la declaración `throws` a la firma del método. |
| 35 | **ClassNotFoundException** | Java | La JVM no puede encontrar la **clase** que se intenta cargar (a menudo en *runtime*). | Verificar el *classpath* y la correcta inclusión de librerías/JARs. |
| 36 | **NoClassDefFoundError** | Java | La JVM **encontró** la clase inicialmente, pero ya no la encuentra durante el uso. | Asegurar que todas las dependencias estén presentes. |
| 37 | **VirtualMachineError** | Java | La JVM ha sufrido un **fallo interno** o se ha quedado sin recursos esenciales. | Puede requerir aumentar la memoria de la JVM. |
| 38 | **UnboundLocalError** | Python | Se referencia una variable **local** antes de que se le asigne un valor. | Inicializar la variable o declararla como `global`/`nonlocal` si es necesario. |
| 39 | **StopIteration** | Python | Se lanza cuando la función `next()` de un **iterador** no tiene más elementos. | Se maneja internamente por los bucles `for`; usar `try-except` si se usa `next()`. |
| 40 | **LookupError** | Python | Clase base para errores de **búsqueda** de claves o índices. | Usar manejo de excepciones para claves o índices que no existen. |
| 41 | **InvalidKeyException** | Java | Una clave usada en criptografía o un mapa **no es válida** o tiene un formato incorrecto. | Asegurar que la clave cumpla con los requisitos de la API. |
| 42 | **SecurityException** | Python | Excepción lanzada por operaciones relacionadas con el **sistema de seguridad**. | Revisar y ajustar los permisos del sistema o del entorno. |
| 43 | **BlockingIOError** | Python | Operación en un *socket* o archivo en **modo no bloqueante** que se bloquearía. | Usar el manejo de excepciones o cambiar la configuración del socket. |
| 44 | **ConnectionRefusedError** | Python | Error de red cuando el intento de conexión es **rechazado** por el destino. | Asegurarse de que el servidor esté activo y escuchando en el puerto correcto. |
| 45 | **EOFError** | Python | La función `input()` o un archivo alcanza el **fin del archivo** inesperadamente. | Manejar la entrada de datos o verificar que el archivo no esté vacío. |
| 46 | **KeyboardInterrupt** | Python | El usuario **interrumpe** la ejecución (generalmente con Ctrl+C). | Usar `try-except` para realizar una limpieza antes de salir. |
| 47 | **OSError** | Python | Excepción general del sistema operativo (fallos de E/S, permisos). | Inspeccionar el mensaje de error detallado para determinar el problema del SO. |
| 48 | **ReferenceError** | Python | Un *proxy* de una referencia débil se usa después de que el **objeto ha sido recolectado**. | Evitar el uso de referencias débiles después de que el objeto ha sido eliminado. |
| 49 | **SystemError** | Python | Errores internos del **intérprete** de Python. | Generalmente indica un problema con la instalación de Python o un bug en el intérprete. |
| 50 | **TimeoutError** | Python | Una operación (ej. *socket*) **excede** el tiempo de espera. | Aumentar el tiempo de espera o verificar la carga del recurso. |
| 51 | **ProtocolError** | Python | Un error en el **protocolo** de red o serialización (ej. JSON, HTTP). | Verificar que los datos de entrada/salida cumplen con el formato del protocolo. |
| 52 | **IndentationError** | Python | La **indentación** no es correcta o es inconsistente. | Corregir la indentación para reflejar la estructura de bloques de código. |
| 53 | **DeprecationWarning** | Python | Advertencia de que una función/clase está **obsoleta** y será eliminada. | Reemplazar la función/clase con la alternativa recomendada. |
| 54 | **ThreadDeath** | Java | Una instancia de `Thread` ha sido **detenida** abruptamente (generalmente por `stop()`). | Evitar el uso de `Thread.stop()` y usar mecanismos de terminación cooperativa. |
| 55 | **ReadOnlyFileSystemException** | Java | Se intenta **escribir** en un sistema de archivos montado como **solo lectura**. | Verificar los permisos del sistema de archivos. |
| 56 | **BufferOverflowException** | Java | Se intenta escribir más datos de los que puede contener un **Buffer**. | Verificar la capacidad del `Buffer` antes de la operación de escritura. |
| 57 | **MissingResourceException** | Java | No se puede encontrar un **recurso** (ej. paquete de idioma) en el *classpath*. | Verificar la configuración del *classpath* y la ubicación de los recursos. |
| 58 | **MalformedURLException** | Java | Se intenta crear un objeto `URL` con una cadena de **formato incorrecto**. | Asegurar que la cadena de la URL cumpla con el estándar (protocolo://dominio). |
| 59 | **ConnectException** | Java | Fallo al intentar **conectar** a una dirección y puerto remoto. | Verificar si el servidor está escuchando en ese puerto. |
| 60 | **SQLTimeoutException** | Java | Una operación de base de datos **excede** el tiempo de espera configurado. | Aumentar el *timeout* de la conexión o revisar la consulta SQL. |
| 61 | **SQLException** | Java | Error en la interacción con la **base de datos** (ej. consulta SQL inválida). | Revisar la sintaxis de la consulta SQL y la conexión a la base de datos. |
| 62 | **AWTException** | Java | Un error del sistema o *toolkit* en el **manejo de la interfaz gráfica** (AWT). | Suele estar relacionado con problemas del sistema operativo subyacente. |
| 63 | **UnrecoverableKeyException** | Java | La **clave** criptográfica solicitada no se puede recuperar de un almacén. | Verificar la contraseña o el formato del almacén de claves. |
| 64 | **BadPaddingException** | Java | Los datos cifrados tienen un **relleno incorrecto** al ser descifrados. | Asegurar que se usó el mismo algoritmo de cifrado/descifrado. |
| 65 | **InvalidAlgorithmParameterException** | Java | Los **parámetros** de un algoritmo criptográfico son inválidos. | Revisar los parámetros del algoritmo, como el tamaño de la clave. |
| 66 | **InvalidMimeTypeException** | Java | Se usa un **tipo MIME** que no es válido. | Usar el formato MIME correcto (ej. `application/json`). |
| 67 | **EmptyStackException** | Java | Se intenta extraer o mirar el elemento superior de una **pila** vacía. | Verificar si la pila está vacía antes de la operación (`stack.isEmpty()`). |
| 68 | **NoSuchElementException** | Java | Se intenta obtener el siguiente elemento de un **iterador** que ha terminado. | Verificar `iterator.hasNext()` antes de llamar a `iterator.next()`. |
| 69 | **IllegalAccessException** | Java | Una clase intenta acceder a un campo o método al que **no tiene acceso** (ej. `private`). | Cambiar el modificador de acceso del miembro (ej. a `public`) o usar *Reflection* correctamente. |
| 70 | **InstantiationException** | Java | Se intenta **instanciar** una clase abstracta o una interfaz (usando *Reflection*). | Solo instanciar clases concretas. |
| 71 | **InvocationTargetException** | Java | Excepción lanzada por un método **invocado** a través de *Reflection*. | Desempaquetar la excepción para ver la causa real (`e.getTargetException()`). |
| 72 | **ArrayStoreException** | Java | Intento de almacenar un objeto de tipo **incorrecto** en un array de objetos. | Asegurar que el tipo de objeto sea compatible con el tipo base del array. |
| 73 | **BufferUnderflowException** | Java | Se intenta leer más datos de los disponibles en un **Buffer**. | Verificar la cantidad de datos disponibles antes de leer. |
| 74 | **InvalidPathException** | Java | La **cadena de ruta** de un archivo contiene caracteres inválidos para el SO. | Usar rutas de archivo válidas para el sistema operativo. |
| 75 | **IllegalThreadStateException** | Java | Un método es llamado en un **hilo** que no está en el estado apropiado (ej. llamar `start()` dos veces). | Verificar el estado del hilo antes de la llamada. |
| 76 | **NoSuchFieldException** | Java | Intento de acceder a un **campo** (variable) usando *Reflection* que no existe. | Verificar el nombre y la accesibilidad del campo. |
| 77 | **ClassCastException** | Python | Error común en *type hints* o código que espera una herencia específica. | Corregir la lógica del código o las anotaciones de tipo. |
| 78 | **NotADirectoryError** | Python | Una operación que requiere un **directorio** se aplica a un archivo. | Verificar el tipo de ruta antes de la operación (ej. `os.path.isdir()`). |
| 79 | **IsADirectoryError** | Python | Una operación que requiere un **archivo** se aplica a un directorio. | Verificar el tipo de ruta antes de la operación (ej. `os.path.isfile()`). |
| 80 | **BrokenPipeError** | Python | El **pipe de conexión** se rompe, generalmente cuando un subproceso termina inesperadamente. | Manejar la excepción, a menudo reintentando la operación o limpiando. |
| 81 | **BlockingIOError** | Java | Similar a Python, error en un *socket* o I/O en **modo no bloqueante**. | Usar manejo de excepciones para operaciones no bloqueantes. |
| 82 | **IllegalMonitorStateException** | Java | Un hilo intenta esperar, notificar o notificar a todos **sin ser dueño del monitor** del objeto (`synchronized`). | Asegurar que el método esté `synchronized` o en un bloque `synchronized`. |
| 83 | **MissingServletParameterException** | Java | (Spring/Web) Un **parámetro** requerido en una solicitud web no se proporciona. | Asegurar que la solicitud incluya todos los parámetros definidos. |
| 84 | **HttpMediaTypeNotSupportedException** | Java | (Spring/Web) El **tipo de contenido** (MIME) enviado por el cliente no es aceptado. | Asegurar que el encabezado `Content-Type` de la solicitud sea compatible. |
| 85 | **HttpRequestMethodNotSupportedException** | Java | (Spring/Web) Se usa un **método HTTP** (ej. GET) no permitido para esa URL. | Usar el método HTTP correcto (ej. POST, PUT). |
| 86 | **JsonParseException** | Java | Fallo al **analizar (parsear)** una cadena que se supone es JSON válido. | Verificar que el formato de la cadena JSON sea sintácticamente correcto. |
| 87 | **InvalidSessionException** | Java | El usuario intenta acceder a la aplicación con una **sesión inválida** o expirada. | Forzar al usuario a iniciar sesión nuevamente. |
| 88 | **ResourceNotFoundException** | Java | (Spring/Web) Un **recurso** específico (ej. un registro de base de datos) no se encuentra. | Verificar la existencia del recurso antes de intentar acceder a él. |
| 89 | **StaleObjectStateException** | Java | (Hibernate/JPA) Se intenta **actualizar** un objeto que fue modificado por otra transacción. | Implementar control de concurrencia optimista (versiones). |
| 90 | **TransactionRequiredException** | Java | Una operación requiere una **transacción** activa, pero no se proporciona. | Asegurar que el método esté anotado con `@Transactional`. |
| 91 | **LazyInitializationException** | Java | (Hibernate/JPA) Se intenta acceder a una colección o entidad relacionada que es **carga perezosa** después de cerrar la sesión. | Inicializar explícitamente la colección antes de cerrar la sesión. |
| 92 | **LoopingCallError** | Python | Una función se llama a sí misma **recursivamente** sin una condición de parada adecuada. | Definir una condición de parada clara en la función recursiva. |
| 93 | **AsyncIOError** | Python | Error general en operaciones de **entrada/salida asíncronas**. | Manejar errores específicos de la biblioteca asíncrona utilizada. |
| 94 | **JSONDecodeError** | Python | Fallo al **decodificar** una cadena JSON inválida. | Verificar la sintaxis de la cadena JSON de entrada. |
| 95 | **CalledProcessError** | Python | Un **subproceso** ejecutado retorna un código de salida distinto de cero (error). | Inspeccionar la salida del subproceso para depurar la causa del error. |
| 96 | **DeprecationWarning** | Java | Advertencia que indica una API **obsoleta**. | Reemplazar la API obsoleta con la recomendada. |
| 97 | **UnrecoverableKeyException** | Python | (Criptografía) Una **clave** no se puede recuperar de un almacén. | Verificar la contraseña o el formato del almacén de claves. |
| 98 | **SystemExit** | Java | Excepción lanzada por `System.exit()` que indica una **terminación** controlada del programa. | Usar solo para terminar la aplicación de forma controlada. |
| 99 | **FileNotFoundException** | Java | Se intenta acceder a un **archivo** que no existe. | Verificar la ruta o usar `try-catch` con la excepción. |
| 100 | **RemoteException** | Java | Error que ocurre durante una llamada a **método remoto** (RMI). | Verificar la conectividad de la red y el estado del servicio remoto. |
| 101 | **ArithmeticException** | Python | Excepción general que incluye **ZeroDivisionError**. | Manejar la división por cero. |
| 102 | **BufferError** | Python | Errores relacionados con **buffers** (memoria intermedia) en Python. | Asegurar que el tamaño del buffer es adecuado. |
| 103 | **PermissionError** | Python | Error del SO al intentar acceder a un recurso **sin los permisos necesarios**. | Ejecutar el programa con privilegios suficientes o ajustar los permisos del archivo. |
| 104 | **NotImplemented** | Python | El valor devuelto por métodos que **no están implementados**. | Evitar usar la función o implementar el método. |
| 105 | **TypeError** | Java | (Compilación) Error al usar un **tipo** de forma incorrecta (ej. asignación). | Corregir la asignación de tipos de datos. |
| 106 | **NotImplemented** | Java | Excepción lanzada cuando un método aún **no tiene implementación**. | Implementar la lógica del método. |
| 107 | **NoSuchElementException** | Python | El **iterador** no tiene más elementos (similar a `StopIteration`). | Usar `try-except` o verificar la existencia de elementos. |
| 108 | **InvalidAttributeValueException** | Java | Un **atributo** se establece en un valor que está fuera del rango válido. | Validar el valor del atributo antes de establecerlo. |
| 109 | **MethodNotAllowedException** | Java | El **método HTTP** solicitado no está permitido en ese recurso. | Usar el método correcto (GET, POST, etc.). |
| 110 | **BlockingOperationInProgressException** | Java | Una operación **bloqueante** está en progreso y se intenta iniciar otra en el mismo recurso. | Esperar a que la operación anterior finalice o usar modos no bloqueantes. |
