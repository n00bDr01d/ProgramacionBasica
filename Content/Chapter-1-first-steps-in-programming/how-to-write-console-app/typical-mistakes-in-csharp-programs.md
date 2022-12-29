# Errores típicos en programas de C\#

Ahora revisaremos los **errores típicos en los programas de C # de los** principiantes, como falta punto y coma, falta de comillas, falta de paréntesis, mayúsculas incorrectas, etc.

### Escribir fuera del método principal <a href="#writing-outside-if-the-main-method" id="writing-outside-if-the-main-method"></a>

Uno de los errores comunes con los principiantes es **escribir fuera del cuerpo del método**, porque el entorno integrado o el compilador no pueden leer correctamente los comandos dados en el programa. Aquí hay un ejemplo de un programa escrito incorrectamente:`Main()`

```csharp
static void Main(string[] args)
{
}
Console.WriteLine("Hello C#");
```

### Letras mayúsculas incorrectas <a href="#wrong-letter-capitalization" id="wrong-letter-capitalization"></a>

Otro error es cambiar **mayúsculas y minúsculas**, y estas son importantes para llamar a los comandos y su correcto funcionamiento. Aquí hay un ejemplo de tal error:

```csharp
static void Main(string[] args)
{
    Console.Writeline("Hello C#");
}
```

En el ejemplo anterior está escrito mal y tiene que ser corregido a .`WritelineWriteLine`

### Falta punto y coma <a href="#missing-semicolon" id="missing-semicolon"></a>

La ausencia de **un punto y coma** () al final de los comandos es uno de los eternos problemas del programador principiante. Omitir este signo conduce a **un funcionamiento incorrecto del programa** y**, a menudo, el problema pasa desapercibido**. Aquí hay un ejemplo de un código erróneo:`;`

```csharp
static void Main(string[] args)
{
    Console.Writeline("Hello C#")
}
```

### Falta o es incorrecto entre comillas o paréntesis <a href="#missing-or-wrong-quotation-mark-or-parenthesis" id="missing-or-wrong-quotation-mark-or-parenthesis"></a>

La falta de **comillas** o **la ausencia de paréntesis de apertura o cierre** también pueden ser un problema. Al igual que el punto y coma, aquí también el problema conduce a **un funcionamiento incorrecto del programa** o, en general, a su falla. Este error apenas se nota en un código más grande. Aquí hay un ejemplo de un programa con errores:

```csharp
static void Main(string[] args)
{
    Console.WriteLine("Hello C#);
}
```

Este programa arrojará **un error en tiempo** de compilación y la compilación va a fallar, e incluso antes de eso, el código se subrayará, para señalar al programador el error que cometió (la comilla de cierre faltante):

![](https://csharp-book.softuni.org/assets/chapter-1-images/01.Hello-csharp-08.png)

Falta otro ejemplo o . Puede producir mensajes de error inesperados, no siempre fáciles de entender.`{}`

```csharp
class Example
{
    static void Main(string[] args)
    {
        Console.WriteLine("Hello C#);
}
```
