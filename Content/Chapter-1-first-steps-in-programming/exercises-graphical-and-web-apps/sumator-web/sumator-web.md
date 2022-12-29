# Laboratorio: Aplicación Web "Summator" (Calculadora)

Ahora vamos a crear algo aún más complejo, pero también más interesante: Aplicación web que **calcula la suma de dos números**. Al **introducir dos números** en los dos primeros campos de texto y pulsar el botón \[**Calcular**], **se calcula su suma** y el resultado se muestra en el tercer campo de texto.

Preste atención a que estamos creando **una aplicación basada en la Web**. Esta es una aplicación que está disponible a través de un navegador web, al igual que su correo electrónico favorito o sitio web de noticias. La aplicación web va a tener un lado servidor (back-end), que está escrito en el lenguaje C # con la tecnología MVC ASP.NET, y un lado cliente (front-end), que está escrito en el lenguaje HTML (este es un lenguaje para la visualización de información en un navegador web).

Se espera que la **aplicación web** tenga un aspecto similar al siguiente:

![](https://csharp-book.softuni.org/assets/chapter-1-images/08.Numbers-sum-web-01.png)

Como diferencia en comparación con las aplicaciones de consola, que leen y escriben los datos en forma de texto en la consola, las aplicaciones web tienen **una interfaz de usuario basada en web**. Las aplicaciones web **se cargan desde alguna dirección de Internet** (URL) a través de un navegador web estándar. Los usuarios escriben datos de entrada en una página, visualizados desde el navegador web, los datos se procesan en un servidor web y los resultados se muestran nuevamente en una página del navegador web. Para nuestra aplicación web vamos a utilizar **la tecnología ASP.NET MVC**, que permite crear **aplicaciones web con el lenguaje de programación C# en el** entorno de desarrollo **Visual Studio**.

### Creación de un nuevo proyecto MVC ASP.NET <a href="#creating-a-new-aspnet-mvc-project" id="creating-a-new-aspnet-mvc-project"></a>

En Visual Studio creamos **un nuevo proyecto de C# de tipo "ASP.NET Web Application"** con el nombre **WebApp**:

![](https://csharp-book.softuni.org/assets/chapter-1-images/08.Numbers-sum-web-02.png)

Elegimos como **tipo** de aplicación: "**MVC"**:

![](https://csharp-book.softuni.org/assets/chapter-1-images/08.Numbers-sum-web-03.png)

### Crear una vista (formulario Web Forms) <a href="#creating-a-view-web-form" id="creating-a-view-web-form"></a>

Encontramos el archivo . **La vista de la página de inicio** de nuestra aplicación web está dentro de ella:`Views\Home\Index.cshtml`

![](https://csharp-book.softuni.org/assets/chapter-1-images/08.Numbers-sum-web-04.png)

Eliminamos el código antiguo **del archivo** y escribimos el siguiente código:`Index.cshtml`

![](https://csharp-book.softuni.org/assets/chapter-1-images/08.Numbers-sum-web-05.png)

Este código **crea un formulario web con tres cuadros de texto y un botón**. Dentro de los campos, se están cargando valores, que se calculan previamente en el objeto . El requisito dice que con el clic del botón \[**Calcular**] se llamará a la acción **(acción del controlador).**`ViewBag/home/calculatecalculatehome`

Así es como se supone que **debe verse el archivo** después del cambio:`Index.cshtml`![](https://csharp-book.softuni.org/assets/chapter-1-images/08.Numbers-sum-web-06.png)

### Escribir el código del programa <a href="#writing-the-program-code" id="writing-the-program-code"></a>

Lo que queda es escribir **la acción** que **suma los números al hacer clic en el botón** \[**Calcular**]. Abrimos el archivo y agregamos el siguiente código en el cuerpo de la clase:`Controllers\HomeController.csHomeController`

![](https://csharp-book.softuni.org/assets/chapter-1-images/08.Numbers-sum-web-07.png)

Este código implementa la acción "**calcular**". Toma dos parámetros y los registra en los objetos, después **de lo cual calcula y registra** su suma. Los valores registrados en se utilizan desde la vista, para que se muestren en los **tres campos de texto** dentro del formulario para sumar números en la página web de **la** aplicación.`num1num2ViewBagViewBag`

Así es como debería verse **el archivo** después del cambio:`HomeController.cs`

### Prueba de la aplicación <a href="#testing-the-application" id="testing-the-application"></a>

La aplicación está lista. Podemos iniciarlo con \[**Ctrl+F5**] y probar si funciona:

![](https://csharp-book.softuni.org/assets/chapter-1-images/08.Numbers-sum-web-09.png)

¿Da miedo? **¡No tengas miedo!** Tenemos mucho más que aprender, para alcanzar el nivel de conocimiento y habilidades para escribir aplicaciones basadas en web libremente como en el ejemplo anterior, así como otras mucho más grandes y mucho más complejas. Si no tienes éxito, no hay nada de qué preocuparse, sigue adelante. Después de algún tiempo, recordará con una sonrisa lo incomprensible y emocionante que fue su primera colisión con la programación web.&#x20;

El propósito de los dos ejemplos anteriores (aplicación gráfica de escritorio y aplicación web) no es enseñarle, sino hacer que se sumerja un poco más profundamente en la programación, **para aumentar su interés** hacia el desarrollo de software e inspirarlo a aprender mucho. **Todavía tienes mucho que aprender**, pero es interesante, ¿no?
