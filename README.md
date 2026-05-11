
# Trabajo Práctico: POO en JavaScript

## Cómo ejecutar este proyecto
1. Asegúrate de tener **Node.js** instalado en tu sistema.
2. Abre tu terminal en la ruta de este repositorio.
3. Corre el siguiente comando:
   ```bash
   node actividad.js

## Conceptos Clave de la Clase
¿Qué es la POO?
Es una forma de programar (paradigma) donde modelamos la realidad creando "objetos". Estos objetos tienen características (propiedades) y cosas que pueden hacer (métodos).

La particularidad de JavaScript
A diferencia de lenguajes como Java o C#, JS no tiene clases reales en su núcleo. Funciona a través de prototipos. Cuando usamos class hoy en día, en realidad estamos usando una sintaxis más amigable (azúcar sintáctico) para manejar prototipos por detrás.

Cadena de Prototipos
Es el mecanismo por el cual un objeto hereda propiedades de otro. Si JS no encuentra un método en tu objeto, lo busca en su prototipo, y luego en el prototipo de su prototipo, hasta llegar a null.

## Los 4 Pilares

Encapsulación:
Mantener datos y funciones seguros y agrupados dentro de un objeto.

Abstracción:
Ocultar el código complejo interno y mostrar solo lo que el usuario necesita usar.

Herencia: Crear nuevas clases a partir de otras existentes para no repetir código.

Polimorfismo: Un mismo método puede reaccionar distinto dependiendo del objeto que lo llame.

## Cuestionario de Estudio
Preguntas Conceptuales
¿Qué es un objeto en JavaScript?
Es una colección independiente de variables (propiedades) y funciones (métodos) estructurada en pares de clave y valor.

¿Qué diferencia hay entre clase y objeto?
La clase es el plano arquitectónico y el objeto es la casa construida usando ese plano.

¿Qué es un prototipo?
Un objeto base oculto que actúa como "padre", desde el cual otros objetos pueden heredar características.

¿Qué hace la palabra new?
Reserva memoria para un nuevo objeto en blanco, vincula la palabra this a ese objeto y lo enlaza automáticamente a su prototipo.

¿Por qué JS no es realmente orientado a clases?
Porque su motor interno sigue usando delegación de prototipos en lugar de la herencia estricta basada en clases de la POO tradicional.

Preguntas Técnicas
¿Diferencia entre método en constructor vs en prototype?
Si lo pones en el constructor, cada objeto nuevo crea su propia copia del método (gasta más memoria). Si lo pones en el prototipo, todos los objetos comparten esa única función.

¿Qué hace extends?
Le indica a JavaScript que una clase secundaria va a heredar de una clase principal.

¿Para qué sirve super()?
Es obligatorio usarlo en la clase hija para poder llamar y ejecutar el constructor de la clase padre.

Pensamiento Analítico
¿Cuándo usar POO?
Es ideal para proyectos medianos o grandes donde tienes entidades claras (como Usuarios, Facturas, Productos) que interactúan entre sí.

¿Qué ventaja tiene sobre el código secuencial?
Evita el código espagueti. Es mucho más fácil de mantener, leer y escalar en el futuro.

¿Qué problema resuelve la herencia?
Evita que escribas la misma lógica mil veces (principio DRY: Don't Repeat Yourself)
