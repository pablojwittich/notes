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
- Un *programa* es una clase que contiene el método *main*
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
Un IDE es una herramienta que permite editar programas, compilarlos, depurarlos, documentarlos, ejecutarlos, etc.

### 1.3. Estrucuturas de Control
#### 1.3.1 Entrada y salida de datos por consola 
Llamamos consola al conjunto compuesto por la pantalla (a modo de texto) y el teclado de la computadora donde se ejecutaran nuestros programas.
La *Clase Scanner* permite leer datos ingresado por el teclado. Ej:
~~~
package libro.cap01;
import java.util.Scanner // Agregamos esta para que podamos utilizar la clase Scanner
public class HolaMundoNombre
{
    public static void main (String[] args)
    {
        Scanner scan = new Scanner(System.in);
        System.out.print("Ingrese su nombre");
        String nom = Scanner.nextline();
        System.out.println("Hola Mundo! " + nom);
    }
}
~~~



