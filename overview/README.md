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

Several commands can be written as a sequence, called "**computer program**":

```csharp
var size = 5;
Console.WriteLine("Size = " + size);
Console.WriteLine("Area = " + size * size);
```

Run the above code example: [https://repl.it/@nakov/square-area-csharp](https://repl.it/@nakov/square-area-csharp).

The **result** (output) from the above program is as follows:

```
Size = 5
Area = 25
```

The above **program** (sequence of commands) consists of 3 commands:

1. Defines a variable `size` and stores an integer value `5` in it.
2. Prints the value of the variable `a`, along with some text.
3. Calculates and prints the value of the expression `a * a`.

Let's explain in greater detail what is **programming**, what is programing **language**, how to write **commands** and simple **programs** in the **C#** language, using the Visual Studio development environment.
