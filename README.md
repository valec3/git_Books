# Bases de datos

### Definición

Un lugar donde se almacena información de forma organizada

## Tipos

* Bases de datos operativas
* Bases de datos analiticas

## Bases de datos operativas

* Estás bases de datos se utilizan principalmente en OLTP(procesamiento de transacciones en linea), es decir, en situaciones donde existe la necesidad de recopilar, modificar y mantener datos diariamente.
* El tipo de datos almacenados en una base de datos operativa es dinámico

## Bases de datos analiticas

* Se utilizan principalmente en OLAP(procesamiento analítico y en linea) donde existe la necesidad de almacenar y rastrear datos históricos y dependientes del tiempo.
* El tipo de datos almacenados en una base de datos analitica es estático

## Base de datos Relacionales

Almacena datos en tablas

El modelo relacional clasifica las relaciones como uno a uno, uno a muchos, y muchos a muchos.

## Entidades y sus atributos

Una entidad es algo sobre lo que almacenamos información, y los atributos son las datos que describen a esta entidades

Por ejemplo, una entidad del cliente generalmente se describe con un número de cliente, nombre, apellido, calle, ciudad, estado, código postal y número de teléfono.

## Instancias de una entidad cliente en una base de datos.

![](https://learning.oreilly.com/library/view/relational-database-design/9780128499023/B9780128043998000041/B9780128043998000041.xhtml#f0010)

##

##

## identificadores de identidad

Estos nos garantiza que una instancia tiene un identificador único

## Atributos multivalor

Debido a que una entidad en una base de datos relacional no puede tener atributos multivalores, debe manejar esos atributos creando una entidad para mantenerlos.

##

Como regla general, si se encuentra con un atributo multivalor, esta es una pista importante de que necesita otra entidad. La única forma de manejar múltiples valores del mismo atributo es crear una entidad de la cual pueda almacenar múltiples instancias, una para cada valor del atributo

Debido a que una entidad en una base de datos relacional no puede tener atributos multivalor,debe manejar esos atributos creando una entidad para manejarlos

#### Code Blocks (Indented style)

Indented 4 spaces, like `<pre>` (Preformatted Text).

```
<?php
    echo "Hello world!";
?>
```

Code Blocks (Preformatted text):

```
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
```

#### Javascript　

```javascript
function test(){
    console.log("Hello world!");
}
 
(function(){
    var box = function(){
        return box.fn.init();
    };

    box.prototype = box.fn = {
        init : function(){
            console.log('box.init()');

            return this;
        },

        add : function(str){
            alert("add", str);

            return this;
        },

        remove : function(str){
            alert("remove", str);

            return this;
        }
    };
    
    box.fn.init.prototype = box.fn;
    
    window.box =box;
})();

var testBox = box();
testBox.add("jQuery").remove("jQuery");
```

### Images

Image:

![](https://pandao.github.io/editor.md/examples/images/4.jpg)

### Lists

#### Unordered list (-)

* Item A
* Item B
* Item C

\####Unordered list (\*)

* Item A
* Item B
* Item C

#### Unordered list (plus sign and nested)

* Item A
* Item B
  * Item B 1
  * Item B 2
  * Item B 3
* Item C
  * Item C 1
  * Item C 2
  * Item C 3

#### Ordered list

1. Item A
2. Item B
3. Item C

***

### Tables

| First Header | Second Header |
| ------------ | ------------- |
| Content Cell | Content Cell  |
| Content Cell | Content Cell  |

| First Header | Second Header |
| ------------ | ------------- |
| Content Cell | Content Cell  |
| Content Cell | Content Cell  |

| Function name | Description                |
| ------------- | -------------------------- |
| `help()`      | Display the help window.   |
| `destroy()`   | **Destroy your computer!** |

| Item     | Value |
| -------- | ----: |
| Computer | $1600 |
| Phone    |   $12 |
| Pipe     |    $1 |

| Left-Aligned  |  Center Aligned | Right Aligned |
| ------------- | :-------------: | ------------: |
| col 3 is      | some wordy text |         $1600 |
| col 2 is      |     centered    |           $12 |
| zebra stripes |     are neat    |            $1 |

***
