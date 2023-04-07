
# JavaScript

JavaScript es un lenguaje case-sensitive(sensible a MAYUS/MINUS)

online != ONLINE != OnlinE

## Tipos de datos

  

### Primitivos
Son inmutables

* Numbers

* Bool

* Strings

* Floats

* Undefined y Null

### Objetos
Son mutables
* Arrays

* Clases


## Comments

JavaScript supports two styles of comments.

  

```

// This is a single-line comment.

  

/*

*This is a multi-line comment

*and the * characters just look cool!

*/

```

## Unicode

Programmers can use mathematical symbols and words from non-English languages as constants and variables:

```

const π = 3.14

```

  

## Palabras reservadas

  

```

as const export get null target void

async continue extends if of this while

await debugger false import return throw with

break default finally in set true yield

case delete for instanceof static try

catch do from let super typeof

class else function new switch var╔

```

  

## Optional semicolons (OJO)

In JavaScript, you can usually omit the semicolon between two statements if those statements are written on separate lines.

  

More formally (and with three exceptions described a bit later), JavaScript treats a line break as a semicolon if the next nonspace character cannot be interpreted as a continuation of the current statement.

```

lest a

a

=

3

console.log(a)

//JavaScript interprets this like

let a; a = 3 ; console.log(a)

```

En general, si una declaración comienza con `(`, `[`, `/`, `+`, o `-`, existe la posibilidad de que pueda interpretarse como una continuación de La declaración anterior. Declaraciones que comienzan con `/`, `+`, y `-` son bastante raro en la práctica, pero las declaraciones comienzan con `(` y `[` son no es raro en absoluto, al menos en algunos estilos de JavaScript programación. A algunos programadores les gusta poner un punto y coma defensivo en el comienzo de cualquier declaración de este tipo para que continúe funcionando correctamente, incluso si la declaración anterior se modifica y una anterior punto y coma de terminación eliminado:

```

let number=0 // Semicolon omitted here

;[x,x+1,x+3].forEach(console.log) //Defensive ; keeps this statement separate

```

### 3 Exceptions more:

* the `return`, `throw`, `yield`, `break`, and `continue` statements, cualquier salto de linea despues de estas declaraciones es considerado ";"

* ++ , -- deben usarse en la misma linea donde se estan aplicando

* Funciones definidas usando sintaxis concisa “ flecha ”: el `=>` flecha misma debe aparecer en la misma línea que la lista de parámetros.



*

GLOSARY

*  **Literales:** Es un valor de un dato que aparece directamente en el programa

  

```

12 //The number twelve

"hola" //A string of text

```

  

*  **Identificadores:** A JavaScript identifier must begin with a letter, an underscore (`_`), or a dollar sign (`$`). Subsequent characters can be letters, digits, underscores, or dollar signs.

```

variable

$monto

_number

a

```

*  **NAME:**

*  **NAME:**

*  **NAME:**

*  **NAME:**

*  **NAME:**

*  **NAME:**

*  **NAME:**

*  **NAME:**

*  **NAME:**

  

```

```

> Written with [StackEdit](https://stackedit.io/).
