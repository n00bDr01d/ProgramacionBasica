# Ejemplo: crear una aplicación de consola "Hello C#"

\
Ejemplo: crear una aplicación de consola "Hello C#" <a href="#example-creating-a-console-application-hello-c" id="example-creating-a-console-application-hello-c"></a>
----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Vamos a crear nuestro primer **programa de consola** en Visual Studio. Iniciaremos el IDE de Visual Studio, crearemos un nuevo proyecto de C# basado en consola, escribiremos unas pocas líneas de código C# y compilaremos y ejecutaremos el programa. Finalmente, enviaremos nuestro código C # para su evaluación en el sistema automatizado de jueces.

### Vídeo: Aplicación de consola en Visual Studio <a href="#video-console-application-in-visual-studio" id="video-console-application-in-visual-studio"></a>

### Aplicación de consola en Visual Studio: paso a paso <a href="#console-app-in-visual-studio-step-by-step" id="console-app-in-visual-studio-step-by-step"></a>

Ya tenemos Visual Studio y podemos iniciarlo. A continuación, creamos un nuevo proyecto de consola: \[**Archivo**] → \[**Nuevo**] → \[**Proyecto**] → \[**Visual C#**] → \[**Windows**] → \[**Aplicación de consola**].

![](https://csharp-book.softuni.org/assets/chapter-1-images/01.Hello-csharp-01.png)

Establecemos un **nombre significativo** para nuestro programa, por ejemplo:![](https://csharp-book.softuni.org/assets/chapter-1-images/01.Hello-csharp-02.png) Visual Studio va a crear para nosotros **un programa C # vacío**, que tenemos que terminar de escribir (VS Solution con VS Project en él, con el archivo de código fuente de C # en él, con una clase de C # en él, con el método en él).`HelloCSharpMain()`

### Escribir el código del programa <a href="#writing-the-program-code" id="writing-the-program-code"></a>

El código fuente del programa C# está escrito en la sección , entre el paréntesis de apertura y cierre. Este es el método principal (acción) que se ejecuta con el inicio de un programa de C#. Este método se puede escribir de dos maneras:`Main(string[] args){ }Main()`

* `static void Main(string[] args)` – con parámetros de la línea de comandos (no vamos a entrar en detalles)
* `static void Main()` – sin parámetros desde la línea de comandos.

Ambas formas son válidas, ya que **se recomienda la segunda**, porque es más corta y clara. Por defecto, sin embargo, al crear una aplicación de consola, Visual Studio utiliza la primera forma, que podemos editar manualmente si queremos, y eliminar la parte con los parámetros .`string[] args`

Pulse \[**Intro**] después **de los paréntesis de apertura** y **comience a escribir**. El código del programa está escrito **hacia adentro**, ya que esto es una parte de la configuración del texto para mayor comodidad durante una revisión y / o depuración.`{`

![](https://csharp-book.softuni.org/assets/chapter-1-images/01.Hello-csharp-03.png)

Escriba el siguiente comando:

```csharp
Console.WriteLine("Hello C#");
```

Así es como debería verse nuestro programa en Visual Studio:

![](https://csharp-book.softuni.org/assets/chapter-1-images/01.Hello-csharp-04.png)

El comando en el lenguaje C# significa ejecutar la impresión () en la consola () e imprimir el mensaje de texto, que debemos rodear con comillas, para aclarar que se trata de un texto. Al final de cada comando en el lenguaje C# se está poniendo el símbolo y dice que el comando termina en ese lugar (no continúa en la siguiente línea).`Console.WriteLine("Hello C#")WriteLine(…)ConsoleHello C#;`

Este comando es muy típico en la programación: decimos que se debe encontrar un **objeto** determinado (en este caso la consola) y se debe ejecutar alguna **acción** sobre él (en este caso se trata de imprimir algo que se da dentro de los corchetes). Más técnicamente explicado, llamamos al método de la clase y le damos como parámetro un texto literal .`WriteLine(…)Console"Hello C#"`

### Inicio del programa <a href="#starting-the-program" id="starting-the-program"></a>

Para iniciar el programa, pulse \[**Ctrl + F5**]. Si no hay ningún error, se ejecutará el programa. El resultado se escribirá en la consola (en la ventana negra):

![](https://csharp-book.softuni.org/assets/chapter-1-images/01.Hello-csharp-05.png)

Observe que lo iniciamos con **\[Ctrl+F5**], y no solo con **\[F5] o con** el botón de inicio en Visual Studio. Si usamos **\[F5]**, el programa se ejecutará en breve y justo después la ventana negra desaparecerá, y no vamos a ver el resultado.

En realidad, la salida del programa es el siguiente mensaje de texto:

```csharp
Hello C#
```

El mensaje "**Presione cualquier tecla para continuar..."** se muestra adicionalmente en la última línea de la consola después de que finalice el programa, para empujarnos a ver el resultado de la ejecución y presionar una tecla para cerrar la consola.
