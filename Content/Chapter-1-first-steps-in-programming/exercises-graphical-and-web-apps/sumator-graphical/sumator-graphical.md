# Laboratorio: Aplicación gráfica "Summator" (Calculadora)

Escriba una **aplicación gráfica (GUI),** que **calcula la suma de dos números**:

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-01.png)

Al introducir dos números en los dos primeros campos y pulsar el botón \[**Calcular**] se está calculando su suma y el resultado se muestra en el tercer campo de texto. Para nuestra aplicación utilizaremos la **tecnología Windows Forms**, que permite la creación de **aplicaciones gráficas para Windows**, en el entorno de desarrollo **Visual Studio** y con **lenguaje** de programación **C#**.

### Crear un nuevo proyecto de C# <a href="#creating-a-new-c-project" id="creating-a-new-c-project"></a>

En Visual Studio creamos **un nuevo proyecto de C# de tipo "Windows Forms Application"**:

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-02.png)

Al crear una aplicación de Windows Forms se mostrará **un editor para la interfaz de usuario**, en el que se pueden colocar **diferentes elementos visuales** (por ejemplo, cuadros de texto y botones):

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-03.png)

### Agregar campos de texto y un botón <a href="#adding-text-fields-and-a-button" id="adding-text-fields-and-a-button"></a>

Descargamos desde la barra de la izquierda (Caja de herramientas) **tres cuadros de texto** (), **dos etiquetas** () y **un botón** (), luego los organizamos en la ventana de la aplicación. Luego **cambiamos los nombres de cada uno de los controles**. Esto se hace desde la **ventana "Propiedades" a la** derecha, cambiando el campo ():`TextBoxLabelButtonName`

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-04.png)

* Nombres de los cuadros de texto: , , `textBox1textBox2textBoxSum`
* Nombre del botón: `buttonCalculate`
* Nombre del formulario: `FormCalculate`

**Cambiamos los encabezados** (la propiedad) de los controles:`Text`

* `buttonCalculate` -> `Calculate`
* `label1` -> `+`
* `label2` -> `=`
* `Form1` -> `Summator`

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-05.png)

### Cambiar el tamaño de los controles e iniciar la aplicación <a href="#resizing-the-controls-and-starting-the-application" id="resizing-the-controls-and-starting-the-application"></a>

**Redimensionamos y organizamos los controles**, para que se vean mejor:

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-06.png)

Intentamos ejecutar la aplicación \[**Ctrl+F5**]. Debería comenzar, pero no debería **funcionar completamente**, porque aún no hemos escrito lo que sucede cuando hacemos clic en el botón.

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-07.png)

### Escribir el código del programa <a href="#writing-the-program-code" id="writing-the-program-code"></a>

Ahora es el momento de escribir el código, que **suma los números de los** dos primeros campos y **muestra el resultado en el** tercer campo. Para ello, hacemos doble clic en **el botón \[Calcular].** Se mostrará el lugar, en el que escribimos lo que va a suceder haciendo clic en el botón:

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-08.png)

Escribimos el siguiente código C# entre los corchetes de apertura y cierre, donde está el cursor:`{ }`

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-09.png)

Este código toma el **primer** número del campo y lo mantiene en la variable, mantiene el **segundo número** del campo en la variable, después **suma** y en la variable **y** al final **toma el valor de texto de la variable en** el campo. **** `textBox1num1textBox2num2num1num2sumsumtextBoxSum`

### Prueba de la aplicación <a href="#testing-the-application" id="testing-the-application"></a>

Iniciamos el programa de nuevo con \[**Ctrl+F5**] y comprobamos si funciona correctamente. Intentamos calcular 4 + 5, y después **-12.5 + 1.3**:

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-10.png) ![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-11.png)

Intentamos con **números no válidos**, por ejemplo: "**aaa"** y "**bbb**". Parece que hay un problema:

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-12.png) ![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-13.png)

### Corregir el error y volver a probar la aplicación <a href="#fixing-the-bug-and-retesting-the-application" id="fixing-the-bug-and-retesting-the-application"></a>

El problema proviene **de la conversión del campo de texto en un número**. Si el valor dentro del campo **no es un número, el programa produce una excepción**. Podemos reescribir el código para solucionar este problema:

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-14.png)

El código anterior **detecta los errores al trabajar con números** (captura excepciones) y en caso de error **da un valor** en el campo con el resultado. Iniciamos el programa de nuevo con \[**Ctrl+F5**] y probamos si funciona. Esta vez **al ingresar un número incorrecto, el resultado es y el** programa no se rompe:`errorerror`

![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-15.png) ![](https://csharp-book.softuni.org/assets/chapter-1-images/07.Numbers-sum-16.png)

¿Es complicado? Es normal parecer complejo, por supuesto. Estamos empezando a entrar en la programación. El ejemplo anterior requiere mucho más conocimiento y habilidades, que vamos a desarrollar a través de este libro e incluso después. Solo permítete divertirte con la programación de escritorio
