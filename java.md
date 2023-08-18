---
description: Apuntes java
---

# JAVA

### Lenguaje interpretado o compilado

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption><p>Como puede ver en la figura, el código Java comienza su vida como fuente Java legible por humanos, y luego es compilado por <code>javac</code> en un archivo .class y cargado en un JVM. Es común que las clases sean manipuladas y alteradas durante el proceso de carga.</p></figcaption></figure>

* Algunas personas describen el sistema Java como “ compilado dinámicamente. ” Esto enfatiza que la compilación que importa es la compilación JIT en tiempo de ejecución, no la creación del archivo de clase durante el proceso de compilación.
* `javac` no es un compilador en el mismo sentido que `gcc` es — es realmente un generador de archivos de clase para el código fuente de Java. El compilador real en el ecosistema Java es el compilador JIT

Entonces, ¿la respuesta real a “ es Java compilado o interpretado? ” es “ ambos. ” Con la distinción entre lenguaje y plataforma ahora más clara, pasemos a hablar sobre el nuevo modelo de lanzamiento de Java.
