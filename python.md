---
description: Esto es python
---

# Python

## Tokens

#### Identifiers

Un identificador es un nombre utilizado para especificar una variable, función, clase, módulo u otro objeto. Un identificador comienza con una letra (es decir, cualquier carácter que Unicode clasifique como letra) o un guión bajo (\_), seguido de cero o más letras, guiones bajos, dígitos u otros caracteres que Unicode clasifique como letras, dígitos o signos de combinación.

### Literals

A literal is the direct denotation in a program of a data value (a number, string, or container). The following are number and string literals in Python:

```
42                     # Integer literal
3.14                   # Floating-point literal
1.0j                   # Imaginary literal
'hello'                # String literal
"world"                # Another string literal
"""Good
night"""               # Triple-quoted string literal, spanning 2 lines
```

#### Keywords

| **and**    | **break**    | **elif**    | **from**   | **is**       | **pass**   | **with**  |
| ---------- | ------------ | ----------- | ---------- | ------------ | ---------- | --------- |
| **as**     | **class**    | **else**    | **global** | **lambda**   | **raise**  | **yield** |
| **assert** | **continue** | **except**  | **if**     | **nonlocal** | **return** | **False** |
| **async**  | **def**      | **finally** | **import** | **not**      | **try**    | **None**  |
| **await**  | **del**      | **for**     | **in**     | **or**       | **while**  | **True**  |

## Declaraciones

### Declaración simple

Una declaración simple se encuentra completamente dentro de una línea lógica.

Puede colocar más de una simple instrucción en una sola línea lógica, con un punto y coma (;) como separador. Sin embargo, usar una instrucción por línea es el estilo habitual y recomendado de Python, y hace que los programas sean más legibles.

### Declaración compuesta

Una declaración compuesta tiene uno o más cláusulas, alineado en la misma sangría.

Cada cláusula tiene un encabezado comenzando con una palabra clave y terminando con dos puntos (:), seguido de un cuerpo, que es una secuencia de una o más declaraciones.

### Tipos de datos

Los valores de datos en Python se conocen como _objetos_

### Numeros

Todos los números en Python son objetos inmutables; por lo tanto, cuando realiza una operación en un objeto numérico, produce un nuevo objeto numérico.

Los tipos numéricos integrados en Python incluyen enteros, números de coma flotante y números complejos.

```python
1, 23, 3493                    # Decimal integer literals
0b010101, 0b110010, 0B01       # Binary integer literals
0o1, 0o27, 0o6645, 0O777       # Octal integer literals
0x1, 0x17, 0xDA5, 0xda5, 0Xff  # Hexadecimal integer literals
```

```
0., 0.0, .0, 1., 1.0, 1e0, 1.e0, 1.0E0  # Floating-point literals
```

Un valor de punto flotante de Python corresponde a una C doble y comparte sus límites de rango y precisión: típicamente 53 bits — aproximadamente 15 dígitos — de precisión en plataformas modernas.

```
>>> f=2.5
>>> f.as_integer_ratio()
```

<pre><code><strong>( 5, 2 )
</strong></code></pre>

#### Underscores en literales numéricos

```
>>> 100_000.000_0001, 0x_FF_FF, 0o7_777, 0b_1010_1010
```

<pre><code><strong>( 100000.000001, 65535, 4095, 170 )
</strong></code></pre>

### Secuencias

Una _secuencia_ es un contenedor ordenado de artículos, indexado por enteros. Python tiene tipos de secuencia integrados conocidos como cadenas (bytes o str), tuplas y listas.&#x20;

#### Strings

Python tiene dos tipos de cadenas incorporados, str y bytes. El objeto str es una secuencia de caracteres utilizados para almacenar y representar información basada en texto. El objeto bytes almacena y representa secuencias arbitrarias de bytes binarios. Las cadenas de ambos tipos en Python son _inmutable_

```python
'This is a literal string'
"This is another string"
```

```python
the_text = """\
First line
Second line
"""      # The same as "First line\nSecond line\n" but more readable
```

Múltiples literales de cadena de cualquier tipo — cotizados, comillas triples, sin procesar, bytes, formateados — pueden ser adyacentes, con espacios en blanco opcionales entre ( siempre que no mezcle cadenas que contengan texto y bytes ).

```python
marypop = ('supercali'       # '(' begins logical line,
           'fragilistic'     # indentation is ignored
           'expialidocious') # until closing ')'
```

La cadena asignada a marypop es una sola palabra de 34 caracteres.

**Objetos bytes**

Un objeto byte es una secuencia ordenada de ints de 0 a 255. bytes los objetos generalmente se encuentran al leer datos o escribir datos en una fuente binaria (, por ejemplo, un archivo, un socket o un recurso de red ).

Un objeto byte puede ser inicializado  desde una lista de enteros o desde una cadena de caracteres

```python
b'abc'
bytes([97, 98, 99])           # Same as the previous line
rb'\ = solidus'               # A raw bytes literal, containing a '\'
```

#### _<mark style="color:red;">objetos bytearray</mark>_

Un Bytearray es un secuencia mutable ordenada de ints de 0 a 255; como un bytes objeto, puedes construirlo a partir de una secuencia de ints o caracteres.

```python
ba = bytearray([97, 98, 99])  # Like bytes, can take a sequence of ints
ba[1] = 97                    # Unlike bytes, contents can be modified
print(ba.decode())            # Prints 'aac'
```

### Tuplas

_Una tupla_ es una secuencia ordenada inmutable de elementos. Los elementos de una tupla son objetos arbitrarios y pueden ser de diferentes tipos. Puede usar objetos mutables ( como listas ) como elementos de tupla, pero la mejor práctica es generalmente evitar hacerlo.

Para denotar una tupla, use una serie de expresiones ( los elementos de la tupla ) separados por comas (,); si cada elemento es literal, toda la construcción es un _tuple literal_. Opcionalmente, puede colocar una coma redundante después del último elemento. Puede agrupar elementos de tupla entre paréntesis, pero los paréntesis son necesarios solo cuando las comas tendrían otro significado

```python
100, 200, 300        # Tuple with three items
(3.14,)              # Tuple with one item, needs trailing comma
()                   # Empty tuple (parentheses NOT optional)
```

También puede llamar al tipo incorporado tupla para crear una tupla. Por ejemplo:

```python
tuple('wow')
```

Esto construye una tupla igual a la indicada por el literal de la tupla:

```python
('w', 'o', 'w')
```

### Sets&#x20;

### Diccionarios

### Booleans

hjggytgyu

### Datos extra

Python 3.9 introdujo el concepto de palabras clave suaves, que son palabras clave que son sensibles al contexto. Es decir, son palabras clave de lenguaje para algunas construcciones de sintaxis específicas, pero fuera de esas construcciones se pueden usar como nombres de variables o funciones, por lo que no son reservado palabras.

### Prompt

Una declaración de expresión que ingresa en el pront (> > >) y vincula el resultado a una variable global llamada \_ \_ ( underscore ).





### POO

#### CLASES

* Una clase tiene atributos con nombres arbitrarios que puede vincular y hacer referencia.
* Puede llamar a un objeto de clase como llamaría a una función. La llamada conocida como _instanciación_, devuelve un objeto conocido como _instancia_ de la clase
* Una clase puede _heredar_ de una o más clases, lo que significa que delega a otros objetos de clase la búsqueda de algunos atributos ( incluyendo regular ymétodos de dunder ) que no están en la clase misma.

<pre class="language-python"><code class="lang-python"><strong>class Classname(base-classes, *, **kw):
</strong>    statement(s)
</code></pre>

Python aconseja el uso de mayúsculas para nombres de clase, como Artículo, PrivilegedUser, MultiUseFacility, etc.

#### Atributos de objetos de clase.

<pre class="language-python"><code class="lang-python"><strong>class C1:
</strong>    x = 23
print(C1.x)                      # prints: 23b
</code></pre>

<pre class="language-python"><code class="lang-python"><strong>class C2:
</strong><strong>    pass
</strong>C2.x = 23
print(C2.x)                      # prints: 23
</code></pre>

En declaraciones directamente en el cuerpo de una clase, las referencias a los atributos de clase deben usar un nombre simple, no un nombre completamente calificado. Por ejemplo:

<pre class="language-python"><code class="lang-python"><strong>class C3:
</strong>    x = 23
    y = x + 22                   # must use just x, not C3.x
</code></pre>

Sin embargo, en declaraciones dentro _métodos_ definido en un cuerpo de clase, las referencias a los atributos de clase deben usar un nombre completamente calificado, no un nombre simple. Por ejemplo:

<pre class="language-python"><code class="lang-python"><strong>class C4:
</strong>    x = 23
<strong>    def amethod(self):
</strong>        print(C4.x)              # must use C4.x or self.x, not just x!
</code></pre>

#### Metodos

<pre class="language-python"><code class="lang-python"><strong>class C5:
</strong><strong>    def hello(self):
</strong>        print('Hello')
</code></pre>

Además, un método definido en un cuerpo de clase tiene un primer parámetro obligatorio, convencionalmente siempre nombrado _<mark style="color:yellow;">**SELF**</mark>_, que se refiere a la instancia en la que llama al método.

### Instancias

Para crear una instancia de una clase, llame al objeto de clase como si fuera una función. Cada llamada devuelve una nueva instancia cuyo tipo es esa clase:

```python
juan = Persona()
```

La función incorporada isinstance (_yo_, _C_), con una clase como argumento _C_, devuelve **Verdadero** cuando _yo_ es una instancia de clase _C_ o cualquier subclase de _C_. De lo contrario, isinstance devoluciones **Falso**

#### \_\_init\_\_

Cuando una clase define o hereda un método llamado **init**, llamando al objeto de clase ejecuta **init** en la nueva instancia para realizar por instancia de inicialización.

<pre class="language-python"><code class="lang-python"><strong>class Persona:
</strong><strong>    def __init__(self, nombre):
</strong>        self.x = nombre
        
#Crear una instancia de persona
persona_1 = Persona("Mario")
</code></pre>

### Herencia

Crear una instancia establece dos atributos de instancia. Por cualquier caso _z_, _z._\_\_clase\_\_ es el objeto de clase al que _z_ pertenece y _z._\_\_dict\_\_ es el mapeo _z_ usa para mantener sus otros atributos. Por ejemplo, por ejemplo z acabamos de crear:

```python
print(z.__class__.__name__, z.__dict__)  # prints: C7 {'x':23}
```















### Datos extra

​Python 3.9 introdujo el concepto de palabras clave suaves, que son palabras clave que son sensibles al contexto. Es decir, son palabras clave de lenguaje para algunas construcciones de sintaxis específicas, pero fuera de esas construcciones se pueden usar como nombres de variables o funciones, por lo que no son palabras reservadas

En Python, las clases son objetos ( valores ), manejados al igual que otros objetos. Puede pasar una clase como argumento en una llamada a una función, y una función puede devolver una clase como resultado de una llamada. Puede vincular una clase a una variable, un elemento en un contenedor o un atributo de un objeto. Las clases también pueden ser claves en un diccionario. Como las clases son objetos perfectamente comunes en Python, a menudo decimos que las clases son _primera clase_ objetos.

Un \_\_init\_\_ el método no debe devolver un valor que no sea **Ninguno**; si lo hace, Python plantea un TypeError excepción.



### &#x20;

l​\

