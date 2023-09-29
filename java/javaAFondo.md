# JAVA A FONDO - ING PABLO A. SZNAJDLERDER
---
## 1. Introducción
El lenguaje Java se carateriza por:
- Un lenguaje de propositos generales 
- Fuertemente tipado
- Orientado a objetos
- Creador: James Glosing

### 1.2. Comenzando a programar 
Crearemos un programa que imprima "Hola Mundo!". Antes tenemos que saber que:
- Un **programa** es una clase que contiene el método **main**
- Los bloques de codigo se delimitan por llave {}
- Las sentencias finalizan con ;
- Cada clase debe estar dentro de un archivo de extensión .java y con el mismo nombre que la clase.
~~~
package libro.cap01;
public class HolaMundo
{
    public static void main (String[] args)
    {
        System.out.println("Hola Mundo!");
    }
}
~~~
#### 1.2.1. IDE
Un IDE es una herramienta que permite editar programas, compilarlos, depurarlos, documentarlos, ejecutarlos, etc
### 1.3. Estrucuturas de Control
#### 1.3.1 Entrada y salida de datos por consola 
Llamamos consola al conjunto compuesto por la pantalla (a modo de texto) y el teclado de la computadora donde se ejecutaran nuestros programas.
La **Clase Scanner** permite leer datos ingresado por el teclado. Ej:
~~~
package libro.cap01;
import java.util.Scanner // Agregamos esta para que podamos utilizar la clase Scanner
public class HolaMundoNombre
{
    public static void main (String[] args)
    {
        Scanner scan = new Scanner(System.in);
        System.out.print("Ingrese su nombre");
        String nom = scan.nextline();
        System.out.println("Hola Mundo! " + nom);
    }
}
~~~
#### 1.3.2. Definición de Variables
Podemos definir las variables en cualquier lugar del codigo teniendo en cuenta el **scope** de la misma.
#### 1.3.3. Comentarios en el codigo
Java soporta dos tipos de comentarios:
- De una linea -> //
- De multiples lineas -> /* */
#### 1.3.4. Estructuras de Decisión
Java dispone de 3 estructuras de decisión:
- Decisión simple -> **if**
- Decisión multiple -> **switch**
- Decisión in-line -> **a>b**

**Sintaxis sentencia IF**

Ejemplo
~~~
package libro.cap01;
import java.util.Scanner;

public Class SentenciaIF
{
    public static void main(String[] args)
    {
        Scanner scan = new Scanner(System.in)e
        System.out.print("Ingrese su edad")
        int edad = scan.nextline();

        if (edad > 18)
        {
            System.out.println("Ud. es mayor de edad");
        }
            else
            {
                System.out.println("Ud. es menor de edad");
            }
    }
}
~~~

**Sintaxis sentencia Switch**

Ejemplo
~~~
package libro.cap01;
import java.util.Scanner;

public class SentenciaSwitch
{
    public static void main(String[] args)
    {
        Scanner scan = new Scanner(System.in);
        System.out.print("Ingrese un numero de la semana");
        int v = scan.nextline();
        String dia;

        Switch(v)
        {
            case 1:
                dia = "Lunes";
                System.out.print("Hoy es " + dia);
                break;
            case 2:
                dia = "Martes";
                System.out.print("Hoy es " + dia);
                break;
            case 3:
                dia = "Miercoles";
                System.out.print("Hoy es " + dia);
                break;
            case 4:
                dia = "Jueves";
                System.out.print("Hoy es " + dia);
                break;
            case 5:
                dia = "Viernes";
                System.out.print("Hoy es " + dia);
                break;
            case 6:
                dia = "Sabado";
                System.out.print("Hoy es " + dia);
                break;
            case 7:
                dia = "Domingo";
                System.out.print("Hoy es " + dia);
                break;
            default:
                dia = "Dia incorrecto, ingrese un numero del 1 al 7;
                break;
        }
    }
}
~~~
#### 1.3.5. Estructuras iteractivas 
Disponemos de 3 estructuras: 
- While
- Do While 
- For

**Sintaxis While** 
En este ciclo itera mientras que la condición se *true*
~~~
package libro.cap01;
import java.util.Scanner;

public class EstWhile
{
    public static void main (String[] args)
    {
        Scanner scan = new Scanner(System.in);
        int n = scan.nextline();

        while(i < n)
        {
            //muestro el valor de i
            System.out.print(i);
            //incremento el valor de i
            i++;
        }
    }
}
~~~

**Sintaxis Do-While**
~~~
package libro.cap01;
import java.util.Scanner;

public class EstDoWhile
{
    public static void main (String[] args)
    {
        Scanner = new Scanner(System.in);
        int n = scan.nextline();
        int i = 1;

        do
        {
            System.out.println(i);
            i++;
        }
        while(i <= 1)
    }
}
~~~

**Sintaxis Ciclo for**
~~~
package libro.cap01;
import java.util.Scanner;

public class CicloFor
{
    public static main void(String[] args)
    {
        Scanner scan = new Scanner(System.in);
        int n = nextline();

        for (int i = 1; i <= n; i++)
        {
            System.out.println(i);
        }
    }
}
~~~
### 1.4. Otros elementos del lenguaje
#### 1.4.1 Tipos de Datos

| Tipo  | Descripción           | Longitud |
--------|-----------------------|----------|
| byte  | entrero con signo     | 1 byte   |
| char  | entero sin signo      | 2 bytes  |
| short | entero con signo      | 2 bytes  |
| int   | entero con signo      | 4 bytes  |
| long  | entero con signo      | 8 bytes  | 
| float | punto flotante        | 4 bytes  |
| double| punto flotante        | 8 bytes  |
|boolean| Obj. Logico (t or f)  | 1 byte   |
| String| Obj.                  |          |

*En Java no existe **unsigned** como en C. Por esta razón, los tipos de datos enteros no adminten valores negativos.*

#### 1.4.2. Definición de constantes
Las constantes se definen fuera de los métodos utilizando el modificador final. Por lo general se definen como public and static.

#### 1.4.3. Arrays

    



