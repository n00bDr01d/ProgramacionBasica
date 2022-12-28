# Capítulo 1. Primeros pasos en la programación

En este capítulo, vamos a descubrir **qué es la programación** en su núcleo y cómo escribir programas y aplicaciones simples.

* Nos familiarizaremos con la idea de **lenguajes de programación** y plataformas de desarrollo, junto con conceptos como **compilación** y **ejecución** de código.
* Vamos a ver los **entornos para el desarrollo de software** (IDE) y cómo trabajar con ellos, en particular con **Visual Studio**.
* Escribiremos y ejecutaremos nuestro **primer programa** con el lenguaje de programación **C#** en **Visual Studio**.
* **Haremos ejercicio** con un par de tareas: crearemos programas **basados en consola**, una aplicación gráfica (**GUI)** y una aplicación **Web**.
* Aprenderemos cómo verificar la exactitud de las soluciones de este libro en **el sistema de jueces de SoftUni**.
* Conoceremos algunos de los **errores típicos**, que a menudo se cometen durante la escritura de código y cómo evitar cometerlos.

## Introducción a la codificación por ejemplos <a href="#introduction-to-coding-by-examples" id="introduction-to-coding-by-examples"></a>

Codificación significa escribir **comandos** para la computadora, por ejemplo:

{% code lineNumbers="true" %}
```csharp
Console.WriteLine("Esto es Esparta !!");
```
{% endcode %}

Cuando se ejecuta se muestra lo siguiente:

```
Esto es Esparta !!
```

Se pueden escribir varios comandos como una secuencia, llamada "**programa de computadora**":

```csharp
var size = 5;
Console.WriteLine("Size = " + size);
Console.WriteLine("Area = " + size * size);
```

Ejecuta el anterior código en :  [https://repl.it/@nakov/square-area-csharp](https://repl.it/@nakov/square-area-csharp).

El **resultado** (salida) del programa anterior es el siguiente:

```
Size = 5
Area = 25
```

El **programa** anterior (secuencia de comandos) consta de 3 comandos:

1. Define una variable y almacena un valor entero en ella `zise 5`
2. Imprime el valor de la variable `area`, junto con algún texto.
3. Calcula e imprime el valor del resultado del cálculo `area * area`.

Vamos a explicar con mayor detalle qué es la **programación**, qué es el lenguaje de programación, cómo escribir **comandos** y **programas** simples en el **lenguaje** **C#**, utilizando el entorno de desarrollo de Visual Studio.
