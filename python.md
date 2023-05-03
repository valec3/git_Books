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

###

### Numeros

### Secuencias

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

