# Entornos de desarrollo (IDE) y Visual Studio

Como ya se ha dicho, para programar necesitamos un **Entorno de Desarrollo Integrado** (IDE). Este es en realidad un editor para programas, en el que escribimos el código del programa y podemos compilarlo y ejecutarlo para ver los errores, corregirlos e iniciar el programa nuevamente.

* Para programar con C# usamos **Visual Studio** IDE para el sistema operativo Windows y **MonoDevelop** o **Raider** para Linux o Mac OS X.
* Si programamos con Java, los entornos **IntelliJ IDEA**, **Eclipse** o **NetBeans** son adecuados.
* Si escribimos en Python, podemos usar el entorno **PyCharm**.

### Instalación de Visual Studio <a href="#installing-visual-studio" id="installing-visual-studio"></a>

Comenzamos con la instalación del entorno integrado **Microsoft Visual Studio** (Comunidad, versión 2017, última a partir de junio de 2017). La instalación de versiones posteriores de Visual Studio (como Visual Studio 2019 y Visual Studio 2021) debe ser muy similar.

La versión **Community** de Visual Studio (VS) se distribuye gratuitamente por Microsoft y se puede descargar desde: [https://www.visualstudio.com/vs/community](https://www.visualstudio.com/vs/community).

![](https://csharp-book.softuni.org/assets/chapter-1-images/00.visual-studio-0.png)

La instalación es típica de Windows con \[**Siguiente**], \[**Siguiente**] y \[**Finalizar**], pero es importante incluir los componentes para "**desarrollo de escritorio**" y "**ASP.NET**". No es necesario cambiar el resto de la configuración para la instalación.

Las siguientes líneas describen en detalle **los pasos para la instalación de Visual Studio** (versión Community 2017). Después de descargar el archivo de instalación e iniciarlo, aparece la siguiente pantalla:

![](https://csharp-book.softuni.org/assets/chapter-1-images/00.visual-studio-1.png)

Presione el botón \[**Continuar**] y verá la pantalla debajo:

![](https://csharp-book.softuni.org/assets/chapter-1-images/00.visual-studio-2.png)

Se está cargando una pantalla con el panel de instalación de Visual Studio.

![](https://csharp-book.softuni.org/assets/chapter-1-images/00.visual-studio-3.png)

Ponga una marca de verificación en \[Desarrollo de **la plataforma universal de Windows**], \[Desarrollo **de escritorio .NET**] y \[**Desarrollo ASP.NET y web] y**, a continuación, pulse el botón \[**Instalar**]. Básicamente, esto es todo. ![](https://csharp-book.softuni.org/assets/chapter-1-images/00.visual-studio-4.png)Comienza la instalación de Visual Studio y aparecerá una pantalla como la siguiente:![](https://csharp-book.softuni.org/assets/chapter-1-images/00.visual-studio-5.png)Después de instalar Visual Studio, aparecerá una pantalla informativa. Pulse el botón \[**Iniciar**] para iniciarlo. ![](https://csharp-book.softuni.org/assets/chapter-1-images/00.visual-studio-6.png)Al **iniciar VS** aparece una pantalla como la de abajo. En él, puede elegir si ingresará a Visual Studio con una cuenta de Microsoft. Por ahora, elegimos continuar sin haber iniciado sesión en nuestra cuenta de Microsoft y, por lo tanto, elegimos la opción \[**No ahora, tal vez más tarde].** En un momento posterior, si tiene una cuenta de este tipo, puede iniciar sesión, y si no tiene una, y tiene dificultades con su creación, siempre puede pedir ayuda en el **foro de discusión** oficial de SoftUni ([https://www.reddit.com/r/softuni](https://www.reddit.com/r/softuni)) o en la página oficial de **Facebook** de SoftUni ([https://fb.com/softuni.org](https://fb.com/softuni.org)).

![](https://csharp-book.softuni.org/assets/chapter-1-images/00.visual-studio-7.png)

El siguiente paso es elegir el **tema de color**, en el que se visualiza Visual Studio. La elección aquí se basa completamente en las preferencias del usuario y no importa qué opción se elija.

![](https://csharp-book.softuni.org/assets/chapter-1-images/00.visual-studio-8.png)

Presione el botón \[Iniciar Visual Studio] y se mostrará la vista principal de **Visual Studio** Community:![](https://csharp-book.softuni.org/assets/chapter-1-images/00.visual-studio-9.png)Eso es todo. Estamos listos para trabajar con Visual Studio.

### Versiones anteriores de Visual Studio <a href="#older-versions-of-visual-studio" id="older-versions-of-visual-studio"></a>

Puede usar versiones anteriores de Visual Studio (por ejemplo, la versión 2015 o 2013 o incluso 2010 o 2005), pero no se **recomienda**, ya que no contienen algunas de las opciones más recientes para el desarrollo, y no todos los ejemplos del libro se ejecutarán de la misma manera.

### Entornos de desarrollo en línea <a href="#online-development-environments" id="online-development-environments"></a>

Existen **entornos alternativos para el desarrollo en línea directamente en** su navegador web. Estos entornos no son muy convenientes, pero si no tiene otra oportunidad, puede comenzar su entrenamiento con ellos e instalar Visual Studio más adelante. Aquí hay algunos enlaces útiles:

* Para el lenguaje C# el sitio .**NET Fiddle** permite la escritura de código y su ejecución en línea: [https://dotnetfiddle.net](https://dotnetfiddle.net/).
* Para Java puede utilizar el siguiente IDE de Java en línea: [https://www.compilejava.net](https://www.compilejava.net/).
* Para JavaScript, puede escribir un código JS directamente en la consola de un navegador determinado cuando presione **\[F12]**.
* El sitio Repl.it proporciona un entorno de codificación en línea para múltiples lenguajes (C #, Java, JS, Python, C ++ y muchos más): [https://repl.it](https://repl.it/).

### Soluciones de proyectos y proyectos en Visual Studio <a href="#project-solutions-and-projects-in-visual-studio" id="project-solutions-and-projects-in-visual-studio"></a>

Antes de empezar a trabajar con Visual Studio, es necesario familiarizarse con los conceptos de una **solución de Visual** Studio y un **proyecto de Visual Studio**, que son una parte inevitable de ella.

![](https://csharp-book.softuni.org/assets/chapter-1-images/VS-solutions-and-projects.png)

**Proyecto de Visual Studio** representa "el **proyecto**" en el que estamos trabajando. Al principio, estas serán nuestras aplicaciones de consola, que vamos a aprender escribiendo con la ayuda del libro actual, los recursos en él y el curso Fundamentos de programación en SoftUni. Con un aprendizaje, tiempo y práctica más profundos, estos proyectos se moverán en la dirección de aplicaciones de escritorio, aplicaciones web y otros desarrollos. Un proyecto en VS **agrupa lógicamente varios archivos** construyendo una aplicación o un componente determinado. Un proyecto de C# contiene uno o más archivos de **código fuente de C#, archivos de** configuración y otros recursos. En cada archivo de código fuente de C#, hay una o más **definiciones de tipos** (clases u otras definiciones). En **las clases** hay **métodos** (acciones), y contienen **una secuencia de comandos**. Suena complicado, pero con proyectos más grandes una estructura como esta es muy conveniente y permite una buena organización de los archivos de trabajo.

La solución de **Visual Studio** representa un contenedor (una **solución** de trabajo), en el que **algunos proyectos están enlazados lógicamente**. El propósito del enlace de estos Proyectos VS es crear una oportunidad para que el código de cualquiera de los proyectos colabore con el código del resto de proyectos VS, para garantizar que la aplicación o el sitio web funcionen correctamente. Cuando el producto o servicio de software que desarrollamos es grande, se construye como una solución VS, y esta solución se divide en **proyectos** (**VS** Projects) y dentro de cada proyecto hay **carpetas con archivos fuente**. Esta organización jerárquica es mucho más conveniente con proyectos más serios (digamos más de 50 000 líneas de código).

Para **proyectos más pequeños**, VS Solutions y VS Projects están **complicando el trabajo**, en lugar de ayudar, pero te acostumbrarás rápidamente.
