¡Claro! Aquí tienes un resumen completo y estructurado del video "Curso Java SE 2024 para empezar (teoría y ejercicios)", basado en la transcripción proporcionada.

---

**Resumen del Curso Java SE 2024 para empezar (Teoría y Ejercicios)**

**Tema Principal del Video:**
El video es un curso introductorio a Java Standard Edition (SE) que cubre desde la instalación de las herramientas necesarias (JDK y Apache NetBeans) hasta conceptos fundamentales de programación como variables, tipos de datos, operadores, estructuras de control (condicionales y repetitivas), arrays, funciones, matrices y manejo de excepciones. Incluye ejercicios prácticos para afianzar los conocimientos.

---

**Parte 1: Introducción (0:00 - 0:30)**

*   **Objetivo del curso:** Proporcionar una base sólida para empezar a programar en Java SE.
*   **Contenido a cubrir:**
    *   Instalación de Java (JDK) y Apache NetBeans (IDE).
    *   Variables y tipos de datos.
    *   Operadores.
    *   Estructuras condicionales.
    *   Estructuras repetitivas (bucles).
    *   Arrays.
    *   Funciones.
    *   Matrices.
    *   Ejercicios prácticos intercalados.
*   **Recursos adicionales:** El código y los ejercicios estarán disponibles en GitHub (enlace en la descripción del video original).

---

**Parte 2: Instalación de Java (JDK) (0:31 - 2:06)**

*   **¿Qué es el JDK?** Java Development Kit. Permite compilar y ejecutar programas Java.
*   **Proceso de descarga:**
    1.  Buscar "Descargar Java jdk" en Google.
    2.  Ir a la página oficial de Oracle.
    3.  Se utilizará la **versión 21** en el curso, pero se menciona que otras versiones también son válidas para el nivel del curso.
    4.  Descargar el instalador correspondiente al sistema operativo (Linux, Mac, Windows).
*   **Proceso de instalación:**
    1.  Ejecutar el instalador descargado.
    2.  Seguir los pasos (principalmente "siguiente y siguiente").
    3.  Se recomienda dejar la ruta de instalación por defecto.
    4.  Esperar a que finalice la instalación y cerrar el instalador.
*   **Verificación de la instalación:**
    1.  Abrir una terminal o símbolo del sistema.
    2.  Ejecutar el comando: `java -version`
    3.  Debería mostrar la versión de Java instalada (ej: "Java version 21...").

---

**Parte 3: Instalación de Apache NetBeans (IDE) (2:07 - 3:45)**

*   **¿Qué es Apache NetBeans?** Un Entorno de Desarrollo Integrado (IDE) utilizado para programar en Java (entre otros lenguajes). Es el IDE que se usará en el curso.
*   **Proceso de descarga:**
    1.  Buscar "Descargar Apache NetBeans" en Google.
    2.  Ir a la página oficial de Apache NetBeans.
    3.  Descargar la última versión disponible (en el video, se muestra NetBeans 20).
    4.  **Nota:** La versión de NetBeans no tiene que coincidir con la versión de Java (ej: NetBeans 20 con Java 21 está bien).
    5.  Seleccionar el instalador para el sistema operativo correspondiente.
*   **Proceso de instalación:**
    1.  Ejecutar el instalador descargado.
    2.  Seguir los pasos: "Siguiente", aceptar términos.
    3.  Permite seleccionar el JDK a utilizar (se usará el JDK 21 instalado previamente, aunque se pueden tener varios JDKs).
    4.  Marcar la opción de buscar actualizaciones (opcional).
    5.  Esperar a que finalice la instalación.
*   **Arrancar Apache NetBeans:**
    1.  Buscar "Apache NetBeans" en el sistema y ejecutarlo.
    2.  Con esto, el IDE está listo para usarse.

---

**Parte 4: Primer Programa "Hola Mundo" (3:46 - 6:43)**

*   **Recomendación de Organización en NetBeans (Project Groups):**
    *   Para evitar acumular muchos proyectos mezclados, se recomienda crear "Project Groups".
    *   En NetBeans: `File > Project Groups > New Group`.
    *   Crear una carpeta para el grupo (ej: `cursoJavaYouTube`) y asignarle un nombre.
*   **Creación de un Nuevo Proyecto "Hola Mundo":**
    1.  En NetBeans, ir a `File > New Project` (o el icono correspondiente).
    2.  **Categorías:** Seleccionar `Java with Maven`.
    3.  **Projects:** Seleccionar `Java Application`. Clic en "Next".
    4.  **Project Name:** Dar un nombre (ej: `HolaMundo`).
    5.  **Project Location:** Especificar la ruta donde se guardará el proyecto (dentro de la carpeta del grupo creado, si se hizo).
    6.  **Group ID, Version, Package:** Se pueden dejar los valores por defecto. El "package" es como una carpeta organizativa en Java (ej: `com.mycompany.holamundo`).
    7.  Clic en "Finish".
*   **Estructura del Proyecto y Código Inicial:**
    *   NetBeans genera una estructura de carpetas y un archivo Java principal (ej: `App.java` si el package era `com.mycompany.app` y el proyecto se llamaba `App`, o `HolaMundo.java` dentro de un paquete `com.mycompany.holamundo`).
    *   El archivo contendrá una clase pública con el mismo nombre que el archivo:
        ```java
        package com.mycompany.holamundo; // Puede variar

        public class App { // O HolaMundo, etc.
            public static void main(String[] args) {
                System.out.println("Hello World!");
            }
        }
        ```
*   **Método `main`:**
    *   `public static void main(String[] args)`: Es el punto de entrada de cualquier aplicación Java. El código dentro de este método es lo primero que se ejecuta.
*   **`System.out.println()`:**
    *   Instrucción para imprimir texto (o valores) en la consola. Lo que esté entre comillas se muestra literalmente.
    *   Modificar el mensaje a: `System.out.println("Hola Mundo");`
*   **Guardar y Ejecutar:**
    *   Guardar los cambios (Ctrl + S). Un nombre de archivo en negrita en NetBeans indica que tiene cambios sin guardar.
    *   **Ejecutar:**
        *   Clic en el botón de "Play" (triángulo verde) en la barra de herramientas.
        *   O clic derecho en el archivo/proyecto y seleccionar "Run".
    *   La salida "Hola Mundo" aparecerá en la ventana "Output" de NetBeans.
    *   **Run again (faster):** Un botón con un triángulo verde y un rayo permite re-ejecutar más rápido si ya se ha compilado.

---

**Parte 5: Variables (6:44 - 10:15)**

*   **¿Qué es una Variable?**
    *   Permite almacenar valores de diferentes tipos para utilizarlos en el programa.
    *   Ejemplos de uso: acumular sumas, guardar datos para mostrar al usuario.
*   **Declaración y Asignación:**
    1.  **Tipo de dato:** Indicar qué tipo de valor almacenará la variable (ej: `int` para números enteros).
    2.  **Nombre de la variable:**
        *   No puede contener espacios.
        *   No debe empezar con números.
        *   No debería empezar con ciertos operadores (+, -, etc.).
        *   Debe ser explicativo. Evitar nombres genéricos como `a`, `b`.
        *   **Convención Camel Case:** Para nombres de variables compuestos por varias palabras, la primera palabra en minúscula y las siguientes con la primera letra en mayúscula (ej: `miPrimeraVariable`). Ayuda a la legibilidad.
    3.  **Operador de Asignación (`=`):** Asigna un valor a la variable.
        *   Ejemplo (declaración y asignación en una línea): `int miPrimeraVariable = 5;`
    4.  **Declaración y Asignación en líneas separadas:**
        ```java
        int otraVariable; // Declaración
        otraVariable = 10; // Asignación
        ```
*   **Mostrar Variables:**
    *   Usar `System.out.println()` concatenando texto con la variable:
        ```java
        System.out.println("El valor es: " + miPrimeraVariable);
        ```
*   **Modificación de Variables:**
    *   El valor de una variable puede cambiar durante la ejecución del programa.
    *   Si se asigna un nuevo valor, la variable tomará ese último valor.
        ```java
        miPrimeraVariable = 5;
        System.out.println(miPrimeraVariable); // Muestra 5
        miPrimeraVariable = 20;
        System.out.println(miPrimeraVariable); // Muestra 20
        ```
*   **Scopes (Ámbitos):** Se mencionan brevemente, se verán más adelante. (El alcance de una variable).

---

**Parte 6: Tipos de Variables (Datos Primitivos y String) (10:16 - 14:52)**

*   **Grupos Principales:**
    *   Números Enteros
    *   Números Reales (con decimales)
    *   Booleanos
    *   Cadenas y Caracteres

*   **Números Enteros:**
    *   **`byte`:** 8 bits. Rango pequeño (-128 a 127). Útil para ahorrar memoria si se sabe que el valor es pequeño.
    *   **`short`:** 16 bits.
    *   **`int`:** 32 bits. El más común para números enteros.
    *   **`long`:** 64 bits. Para números enteros muy grandes. Se le añade una `L` al final del número (ej: `long numeroLargo = 1000000000L;`).
    *   La diferencia principal es el rango de valores que pueden almacenar (optimización de memoria).

*   **Números Reales (Punto Flotante):**
    *   **`float`:** Precisión simple (32 bits). Se le añade una `F` al final del número (ej: `float decimalSimple = 3.14F;`).
    *   **`double`:** Precisión doble (64 bits). Es el tipo decimal por defecto en Java.
    *   **Nota:** Los decimales en Java se escriben con punto (`.`), no con coma.
    *   La diferencia es la precisión (cantidad de decimales que pueden almacenar).

*   **Booleanos:**
    *   **`boolean`:** Solo puede tener dos valores: `true` (verdadero) o `false` (falso).
    *   Como un interruptor (encendido/apagado).
    *   Ej: `boolean esMayorDeEdad = true;`

*   **Cadenas y Caracteres:**
    *   **`String`:**
        *   Para almacenar secuencias de caracteres (texto).
        *   Se escribe entre comillas dobles (ej: `String nombre = "Fernando";`).
        *   **Importante:** `String` en Java no es un tipo primitivo, es una **clase (un objeto)**. Se destaca que su primera letra es mayúscula y en NetBeans puede aparecer en un color diferente a los primitivos. Sin embargo, su uso se ha simplificado para que parezca un primitivo.
    *   **`char`:**
        *   Para almacenar un solo carácter.
        *   Se escribe entre comillas simples (ej: `char inicial = 'F';`).
        *   Puede almacenar un número, que se interpretará según la tabla ASCII (ej: `char letraA = 65;` corresponde a 'A').

*   **Ejemplo en Código:**
    ```java
    // Enteros
    byte numByte = 120;
    short numShort = 30000;
    int numInt = 100000;
    long numLong = 1234567890L;

    // Reales
    float numFloat = 99.99F;
    double numDouble = 123.456;

    // Booleanos
    boolean esVerdadero = true;

    // Cadenas y Caracteres
    String texto = "Hola Java";
    char caracter = 'A';
    char caracterAscii = 65; // Representa 'A'

    System.out.println("Int: " + numInt);
    System.out.println("Long: " + numLong);
    System.out.println("Double: " + numDouble);
    System.out.println("Boolean: " + esVerdadero);
    System.out.println("String: " + texto);
    System.out.println("Char: " + caracter);
    System.out.println("Char (ASCII 65): " + caracterAscii);
    ```

---

**Parte 7: Constantes (14:53 - 16:17)**

*   **¿Qué es una Constante?**
    *   Variables cuyo valor no puede ser modificado una vez que se ha asignado.
    *   Deben tener un valor inicial en su declaración.
*   **Declaración en Java:**
    *   Se utiliza la palabra clave `final` al principio de la declaración de la variable.
    *   **Convención de Nomenclatura:** Se suelen escribir en MAYÚSCULAS, con palabras separadas por guion bajo (`_`) (snake_case).
    *   Ejemplo: `final double IVA = 0.21;`
*   **Intento de Modificación:**
    *   Si se intenta cambiar el valor de una constante después de su inicialización, el compilador generará un error.
        ```java
        final int VALOR_CONSTANTE = 100;
        // VALOR_CONSTANTE = 200; // Esto daría error de compilación
        System.out.println("Valor constante: " + VALOR_CONSTANTE);
        ```
*   **Uso:** Para valores que deben permanecer fijos durante todo el programa (ej: valor del IVA, número PI).

---

**Parte 8: Comentarios (16:18 - 17:37)**

*   **Utilidad:**
    *   Agregar contexto o explicaciones al código.
    *   Inutilizar temporalmente fragmentos de código (para pruebas).
    *   Recomendado para código complejo o difícil de entender.
*   **Tipos de Comentarios en Java:**
    1.  **Comentario de una línea:**
        *   Comienza con `//`.
        *   Todo lo que sigue en esa línea es ignorado por el compilador.
        *   Ej: `// Esto es un comentario de una línea`
    2.  **Comentario de varias líneas (o de bloque):**
        *   Comienza con `/*` y termina con `*/`.
        *   Todo el texto entre estos delimitadores es ignorado.
        *   Ej:
            ```java
            /*
            Esto es un
            comentario de
            varias líneas.
            */
            ```
    3.  **Comentario de Documentación (JavaDoc):**
        *   Comienza con `/**` y termina con `*/`.
        *   Se utiliza para generar documentación automática del código (API docs).
        *   No se profundiza en este tipo en el curso básico.
        *   Ej:
            ```java
            /**
             * Este método suma dos números.
             * @param a El primer número.
             * @param b El segundo número.
             * @return La suma de a y b.
             */
            public int sumar(int a, int b) { /* ... */ }
            ```

---

**Parte 9: Clase `Scanner` (Entrada de Datos por Teclado) (17:38 - 22:25)**

*   **Clase `Scanner`:** Permite leer datos introducidos por el usuario a través del teclado (consola).
*   **Uso Básico:**
    1.  **Importar la clase:** Al principio del archivo Java, se necesita la línea:
        `import java.util.Scanner;`
        (NetBeans suele sugerir y añadir esta importación automáticamente si se usa la clase sin importar).
    2.  **Crear un objeto `Scanner`:**
        `Scanner sn = new Scanner(System.in);`
        *   `sn` es el nombre que se le da al objeto (puede ser cualquier nombre válido, como `teclado`).
        *   `System.in` indica que la entrada se tomará del flujo de entrada estándar (el teclado).
    3.  **Leer diferentes tipos de datos:** El objeto `Scanner` tiene métodos para leer distintos tipos:
        *   `sn.nextInt();` // Lee un entero
        *   `sn.nextDouble();` // Lee un double
        *   `sn.nextLine();` // Lee una línea completa de texto (String)
        *   `sn.next();` // Lee la siguiente palabra (String hasta un espacio)
        *   `sn.nextBoolean();` // Lee un booleano (true o false)
        *   Etc.
*   **Recomendaciones y Consideraciones:**
    *   **Mostrar un mensaje al usuario:** Antes de pedir un dato, es bueno imprimir un mensaje indicando qué se espera (ej: `System.out.println("Introduce tu edad:");`).
    *   **Problemas con Decimales (`nextDouble`) y el Separador Local:**
        *   Por defecto, `Scanner` puede esperar la coma como separador decimal si el sistema está configurado en una región que usa coma (ej: España). Java internamente usa punto.
        *   **Solución:** Configurar el `Scanner` para que use el local de EEUU (que usa punto):
            `sn.useLocale(java.util.Locale.US);`
            Esto asegura que se pueda introducir `10.5` y se lea correctamente.
    *   **Problemas con Cadenas Largas con Espacios (`next()` vs `nextLine()`):**
        *   `sn.next()` lee solo hasta el primer espacio.
        *   `sn.nextLine()` lee la línea entera, incluyendo espacios.
        *   **Problema del delimitador con `next()`:** El delimitador por defecto de `Scanner` es el espacio.
        *   **Solución para leer líneas completas consistentemente (especialmente después de leer números):**
            A veces, después de un `nextInt()`, un `nextLine()` subsiguiente puede leer la nueva línea "vacía" que quedó en el buffer.
            Una forma de manejar esto, si se quiere que el delimitador principal sea el salto de línea para `next()` también:
            `sn.useDelimiter("\n");` (en NetBeans). En Eclipse podría ser `"\r\n"`.
            Esto hace que `sn.next()` también lea hasta el salto de línea, comportándose más como `nextLine()`.
            (El video se enfoca en `useDelimiter("\n")` para que `next()` lea la línea completa.)
*   **Ejemplo de Uso:**
    ```java
    import java.util.Scanner;
    import java.util.Locale; // Para Locale.US

    public class EntradaDatos {
        public static void main(String[] args) {
            Scanner sn = new Scanner(System.in);
            sn.useLocale(Locale.US); // Para usar punto como separador decimal
            // sn.useDelimiter("\n"); // Para que next() lea toda la línea

            System.out.println("Introduce un número entero:");
            int numero = sn.nextInt();
            System.out.println("Número introducido: " + numero);

            System.out.println("Introduce un número decimal (ej: 3.14):");
            double decimal = sn.nextDouble();
            System.out.println("Decimal introducido: " + decimal);

            // Limpiar el buffer antes de leer una línea después de un número
            // si no se usa useDelimiter("\n")
            // sn.nextLine();

            System.out.println("Introduce tu nombre completo:");
            String nombreCompleto = sn.next(); // O sn.nextLine(); si no se usó useDelimiter
            System.out.println("Nombre completo: " + nombreCompleto);

            sn.close(); // Es buena práctica cerrar el Scanner cuando no se usa más
        }
    }
    ```

---

**Parte 10: Mostrar Valores (Formas Adicionales con `System.out`) (22:26 - 25:18)**

*   **`System.out.println(texto);`**
    *   Imprime `texto` y luego añade un salto de línea automático.
    *   Atajo en NetBeans: escribir `sout` y presionar Tab.
*   **`System.out.print(texto);`**
    *   Imprime `texto` pero **no** añade un salto de línea. Las siguientes impresiones continuarán en la misma línea.
    ```java
    System.out.print("Hola ");
    System.out.print("Mundo"); // Imprime "Hola Mundo" en una sola línea
    System.out.println(); // Para añadir un salto de línea manualmente
    ```
*   **`System.out.printf(formato, arg1, arg2, ...);`**
    *   Permite imprimir texto con formato, similar a `printf` en C.
    *   `formato` es una cadena que puede contener texto normal y especificadores de formato.
    *   Especificadores comunes:
        *   `%s`: para Strings.
        *   `%d`: para enteros (decimal).
        *   `%f`: para números de punto flotante (decimales).
            *   `%.2f`: para mostrar un flotante con exactamente 2 decimales.
        *   `%n`: para un salto de línea (independiente de la plataforma).
    ```java
    String nombre = "Ana";
    int edad = 30;
    double altura = 1.658;

    System.out.printf("Nombre: %s, Edad: %d años.%n", nombre, edad);
    // Salida: Nombre: Ana, Edad: 30 años. (con salto de línea)

    System.out.printf("Altura: %.2f metros.%n", altura);
    // Salida: Altura: 1.66 metros. (con salto de línea, redondea)
    ```
    *   `printf` tampoco añade un salto de línea automático al final, a menos que se incluya `%n` en la cadena de formato.
    *   El orden de los argumentos (`arg1, arg2`) debe coincidir con el orden de los especificadores en la cadena de formato.

---

**Parte 11: Ejercicios (Con Soluciones en Vivo)**

*   **Ejercicio 1 (25:19 - 27:23): Pedir nombre y saludar.**
    *   Pide un nombre por teclado.
    *   Muestra un saludo: "Hola [nombre]".
    *   Solución: Usa `Scanner` para leer el nombre (String) y `System.out.println()` para el saludo. Se recuerda `useDelimiter("\n")` para `Scanner`.
*   **Operadores Aritméticos (27:24 - 30:47):**
    *   Repaso de suma (`+`), resta (`-`), multiplicación (`*`), división (`/`), módulo (`%`).
    *   **División Entera:** `10 / 6` da `1` porque ambos son `int`. El resultado es la parte entera.
    *   **Módulo:** `10 % 6` da `4` (el resto de la división).
    *   **División por Cero:** No se puede dividir por cero. Produce una `ArithmeticException`.
    *   Se menciona que el tema de "casting" (conversión de tipos) se verá más adelante para obtener resultados decimales en divisiones de enteros.
*   **Ejercicio 2 (30:48 - 33:54): Calcular precio con IVA.**
    *   Pedir el precio de un producto sin IVA.
    *   Calcular el precio con IVA (21%).
    *   Formatear el resultado para que se muestre con dos decimales.
    *   Solución:
        *   Usar `Scanner` con `useLocale(Locale.US)` para leer el precio (double).
        *   Declarar el IVA como una constante (`final double IVA_PORCENTAJE = 1.21;` o `0.21` y luego sumar).
        *   Cálculo: `precioConIva = precioSinIva * IVA_PORCENTAJE;`
        *   Mostrar con `System.out.printf("El precio final es: %.2f euros%n", precioConIva);`
*   **Operadores Unarios (de Incremento/Decremento) (33:55 - 36:39):**
    *   `++` (incremento), `--` (decremento).
    *   **Postfijo (`variable++`, `variable--`):** El valor de la variable se usa primero en la expresión actual, y *luego* se incrementa/decrementa.
        ```java
        int a = 5;
        System.out.println(a++); // Muestra 5, luego a se convierte en 6
        System.out.println(a);   // Muestra 6
        ```
    *   **Prefijo (`++variable`, `--variable`):** La variable se incrementa/decrementa *primero*, y *luego* su nuevo valor se usa en la expresión actual.
        ```java
        int b = 5;
        System.out.println(++b); // b se convierte en 6, luego muestra 6
        System.out.println(b);   // Muestra 6
        ```
    *   Cuando se usan solos (ej: `a++;` en una línea separada), el efecto final sobre `a` es el mismo para prefijo y postfijo. La diferencia es crucial cuando se usan dentro de expresiones más grandes.
*   **Operadores Lógicos (de Comparación) (36:40 - 39:11):**
    *   Repaso de `>` (mayor que), `<` (menor que), `>=` (mayor o igual), `<=` (menor o igual), `==` (igual a), `!=` (distinto de).
    *   **`!` (NOT lógico):** Invierte un valor booleano (`!true` es `false`, `!false` es `true`).
    *   Siempre devuelven un valor booleano (`true` o `false`).
    *   Ejemplo: `(5 > 10)` es `false`. `!(5 > 10)` es `true`.
*   **Operadores Relacionales (Combinación de Lógicos) (39:12 - 42:43):**
    *   **`&&` (AND lógico):** `true` si ambas condiciones son `true`.
        *   Si la primera condición es `false`, la segunda no se evalúa (cortocircuito).
    *   **`||` (OR lógico):** `true` si al menos una condición es `true`.
        *   Si la primera condición es `true`, la segunda no se evalúa (cortocircuito).
    *   **Prioridad:** `&&` tiene mayor prioridad que `||`. Se pueden usar paréntesis `()` para alterar el orden de evaluación.
        *   `cond1 && cond2 || cond3` se evalúa como `(cond1 && cond2) || cond3`.
*   **Casting (Conversión Explícita de Tipos) (42:44 - 45:10):**
    *   Proceso de convertir un valor de un tipo de dato a otro.
    *   **Ejemplo 1 (División de enteros para obtener decimal):**
        ```java
        int num1 = 10;
        int num2 = 6;
        double resultado = (double) num1 / num2; // resultado es 1.666...
        // (double) num1 convierte num1 a double ANTES de la división.
        // Si no se castea, num1 / num2 sería 1, y luego se convertiría a 1.0.
        ```
    *   **Ejemplo 2 (char a int):**
        ```java
        char letra = 'A';
        int valorAscii = (int) letra; // valorAscii es 65
        ```
    *   **Ejemplo 3 (double a float, necesario si se asigna literal double a float):**
        Un literal decimal como `1.5` es un `double` por defecto.
        ```java
        // float miFloat = 1.5; // Error: posible pérdida de precisión de double a float
        float miFloat = (float) 1.5; // Correcto (casting explícito)
        // O mejor:
        float miFloat2 = 1.5F; // Usar el sufijo F
        ```
*   **Clase `Math` (45:11 - 48:50):**
    *   Proporciona métodos estáticos para operaciones matemáticas comunes. No necesita importación explícita (está en `java.lang`).
    *   `Math.abs(numero)`: Valor absoluto.
    *   `Math.floor(decimal)`: Redondea hacia abajo al entero más cercano (devuelve double). Ej: `Math.floor(5.9)` es `5.0`.
    *   `Math.ceil(decimal)`: Redondea hacia arriba al entero más cercano (devuelve double). Ej: `Math.ceil(5.1)` es `6.0`.
    *   `Math.round(decimal)`: Redondeo estándar al entero más cercano (devuelve `long` para `double`, `int` para `float`). Ej: `Math.round(5.3)` es `5`, `Math.round(5.7)` es `6`.
    *   `Math.pow(base, exponente)`: Potencia. Ej: `Math.pow(2, 3)` es `8.0` (2 elevado a 3).
    *   `Math.sqrt(numero)`: Raíz cuadrada. Ej: `Math.sqrt(25)` es `5.0`.
    *   `Math.clamp(valor, min, max)` (Java 21+): Devuelve `valor` si está entre `min` y `max`. Si `valor < min`, devuelve `min`. Si `valor > max`, devuelve `max`.
    *   Constantes: `Math.PI`, `Math.E`.
*   **Clase `Random` (Generación de Números Aleatorios) (48:51 - 50:23):**
    *   Permite generar números pseudoaleatorios.
    *   **Uso:**
        1.  Importar: `import java.util.Random;`
        2.  Crear objeto: `Random random = new Random();`
        3.  Generar números:
            *   `random.nextInt(bound)`: Entero aleatorio entre `0` (inclusive) y `bound` (exclusive).
            *   `random.nextInt(origin, bound)` (Java 17+): Entero aleatorio entre `origin` (inclusive) y `bound` (exclusive). Para generar entre 1 y 10 (incluido el 10), se usa `random.nextInt(1, 11)`.
            *   `random.nextDouble()`: Double aleatorio entre `0.0` (inclusive) y `1.0` (exclusive).
            *   Y otros para `long`, `float`, `boolean`.
    *   **Importante:** `origin` debe ser menor que `bound` en `nextInt(origin, bound)`.
*   **Estructuras Condicionales `if-else` (50:24 - 51:38):**
    *   `if (condicion) { // código si es true } else { // código si es false }`
    *   Permiten ejecutar diferentes bloques de código según si una condición es verdadera o falsa.
    *   El bloque `else` es opcional.
*   **Ejercicio 3 (51:39 - 54:12): Comprobar si un número es divisible por otro.**
    *   Pedir dos números. Indicar si el segundo es divisible por el primero.
    *   Un número `b` es divisible por `a` si `a % b == 0` (o al revés, según la pregunta: el segundo por el primero -> `num1 % num2 == 0`).
    *   Se pide `num1` y `num2`. La condición es `(num1 % num2 == 0)`.
*   **Ejercicio 4 (54:13 - 57:18): Comprobar si un año es bisiesto.**
    *   Un año es bisiesto si es divisible por 4, EXCEPTO si es divisible por 100, A MENOS QUE también sea divisible por 400.
    *   Condición: `(año % 4 == 0 && año % 100 != 0) || (año % 400 == 0)`
*   **Estructura `else if` (57:19 - 58:27):**
    *   Permite anidar múltiples condiciones sin tener `if` dentro de `if`.
    *   `if (cond1) { ... } else if (cond2) { ... } else if (cond3) { ... } else { ... }`
    *   Se evalúan en orden. La primera que sea `true` ejecuta su bloque, y el resto se omite.
*   **Ejercicio 5 (58:28 - 1:01:42): Indicar el mayor de tres números.**
    *   Pedir tres números. Mostrar cuál es el mayor.
    *   Solución con `if-else if-else`:
        *   `if (n1 >= n2 && n1 >= n3)` -> n1 es el mayor.
        *   `else if (n2 >= n1 && n2 >= n3)` -> n2 es el mayor.
        *   `else` -> n3 es el mayor.
*   **Estructura `switch` (1:01:43 - 1:03:40):**
    *   Alternativa a `if-else if-else` para cuando se compara una variable contra múltiples valores constantes.
    *   Sintaxis tradicional (con `break`):
        ```java
        switch (variable) {
            case valor1: // código para valor1; break;
            case valor2: // código para valor2; break;
            default: // código si no coincide ninguno; break;
        }
        ```
    *   Sintaxis moderna (Java 14+, "arrow syntax"):
        ```java
        switch (variable) {
            case valor1 -> // código para valor1;
            case valor2, valor3 -> // código para valor2 o valor3 (agrupado);
            default -> // código por defecto;
        }
        ```
        Si el bloque de código tiene más de una línea, se usan llaves `{}`.
    *   Se usa un ejemplo de días de la semana.
*   **Ejercicio 6 (1:03:41 - 1:08:38): Calculadora básica.**
    *   Pedir dos operandos (double) y un operador (String: "+", "-", "*", "/").
    *   Realizar la operación.
    *   Manejar división por cero y operador inválido.
    *   Solución con `switch` para el operador. Se usa un booleano `correcto` para controlar si se muestra el resultado o un mensaje de error.
*   **Estructura Repetitiva `while` (1:08:39 - 1:10:09):**
    *   `while (condicion) { // código a repetir }`
    *   El código se repite mientras la condición sea `true`.
    *   La condición se evalúa ANTES de cada iteración.
    *   Importante actualizar la variable de control dentro del bucle para evitar bucles infinitos.
    *   Ejemplo: mostrar números del 1 al 10.
*   **Ejercicio 7 (1:10:10 - 1:13:21): Sumar números hasta introducir -1.**
    *   Pedir números al usuario y sumarlos. El programa termina cuando se introduce -1.
    *   Solución con `while (numero != -1)`. Se inicializa `numero` a un valor que permita entrar al bucle (ej: 0) y `suma` a 0. El orden de pedir el número y sumarlo es importante para no sumar el -1.
*   **Estructura Repetitiva `for` (1:13:22 - 1:14:47):**
    *   `for (inicializacion; condicion; actualizacion) { // código a repetir }`
    *   Generalmente usado cuando se conoce el número de iteraciones.
    *   `inicializacion`: se ejecuta una vez al inicio.
    *   `condicion`: se evalúa antes de cada iteración.
    *   `actualizacion`: se ejecuta después de cada iteración.
    *   Recomendación: `for` para rangos definidos, `while` para rangos no definidos.
    *   Se puede modificar el paso de actualización (ej: `i += 2` para ir de 2 en 2).
*   **Ejercicio 8 (1:14:48 - 1:16:11): Mostrar números del 1 al 100 divisibles por 2 y 3.**
    *   Solución con `for` de 1 a 100. Dentro, un `if (i % 2 == 0 && i % 3 == 0)`.
*   **Ejercicio 9 (1:16:12 - 1:18:13): Mostrar tabla de multiplicar de un número.**
    *   Pedir un número. Mostrar su tabla del 1 al 10.
    *   Solución: pedir el número, luego un `for` de 1 a 10, e imprimir `numero + " x " + i + " = " + (numero * i)`.
*   **Estructura Repetitiva `do-while` (1:18:14 - 1:19:32):**
    *   `do { // código a repetir } while (condicion);`
    *   El código se ejecuta AL MENOS UNA VEZ, porque la condición se evalúa DESPUÉS de la iteración.
    *   Útil para validación de datos (pedir hasta que se introduzca algo correcto).
*   **Ejercicio 10 (1:19:33 - 1:22:06): Validar que un número sea positivo.**
    *   Pedir un número hasta que sea positivo (>= 0 o > 0, según se defina).
    *   Solución con `do-while`. Dentro del `do`, se pide el número. La condición `while` es `(numero < 0)`. Si es negativo, se vuelve a pedir.
*   **Scopes (Ámbitos de Variables) (1:22:07 - 1:24:40):**
    *   Una variable declarada dentro de un bloque de código (delimitado por llaves `{}`) solo existe y es accesible dentro de ese bloque y sus bloques anidados.
    *   No se puede acceder desde fuera del bloque donde se declaró.
    *   Ejemplo: una variable declarada dentro de un `if` no se puede usar después del `if`.
    *   Si se necesita usar una variable en un ámbito más amplio, debe declararse en ese ámbito más amplio.
*   **Clase `String` (Métodos Útiles) (1:24:41 - 1:30:09):**
    *   `cadena.length()`: Devuelve la longitud (número de caracteres) de la cadena.
    *   `cadena.charAt(indice)`: Devuelve el carácter en la posición `indice` (empieza en 0).
    *   `cadena.toLowerCase()`: Convierte la cadena a minúsculas.
    *   `cadena.toUpperCase()`: Convierte la cadena a mayúsculas.
    *   `cadena1.concat(cadena2)`: Concatena `cadena2` al final de `cadena1`. También se puede usar el operador `+`.
    *   `cadena.substring(inicio, finExclusivo)`: Obtiene una subcadena desde `inicio` hasta `finExclusivo - 1`.
    *   `cadena.indexOf(subcadena)`: Devuelve el índice de la primera ocurrencia de `subcadena`, o -1 si no se encuentra.
    *   **Comparación de Strings:**
        *   **NO usar `==` para comparar el contenido de Strings.** `==` compara si son el mismo objeto en memoria, no si tienen los mismos caracteres.
        *   Usar `cadena1.equals(cadena2)`: Devuelve `true` si las cadenas tienen el mismo contenido (sensible a mayúsculas/minúsculas).
        *   Usar `cadena1.equalsIgnoreCase(cadena2)`: Igual que `equals`, pero ignora diferencias de mayúsculas/minúsculas.
    *   **Recorrer un String (carácter a carácter):**
        ```java
        String texto = "Hola";
        for (int i = 0; i < texto.length(); i++) {
            char caracter = texto.charAt(i);
            System.out.println(caracter);
        }
        ```
*   **Ejercicio 11 (1:30:10 - 1:33:53): Contar vocales en una frase.**
    *   Pedir una frase. Contar cuántas vocales (a, e, i, o, u) tiene.
    *   Solución: Convertir la frase a minúsculas (o mayúsculas) para simplificar la comparación. Recorrerla con un `for`. Usar un `switch` (o `if-else if`) para cada carácter y ver si es una vocal, incrementando un contador.
*   **Ejercicio 12 (1:33:54 - 1:38:19): Contar mayúsculas y minúsculas.**
    *   Pedir una frase. Contar cuántas letras mayúsculas y cuántas minúsculas tiene.
    *   Truco con la tabla ASCII: Las letras mayúsculas ('A'-'Z') y minúsculas ('a'-'z') tienen rangos de valores numéricos contiguos.
    *   Se puede comparar un `char` como si fuera un número:
        `if (caracter >= 'A' && caracter <= 'Z') { // es mayúscula }`
        `else if (caracter >= 'a' && caracter <= 'z') { // es minúscula }`
*   **Ejercicio 13 (1:38:20 - 1:40:56): Eliminar espacios de una frase.**
    *   Pedir una frase. Crear una nueva frase sin espacios.
    *   Solución: Recorrer la frase original. Si el carácter actual no es un espacio, concatenarlo a la nueva frase.
*   **Ejercicio 14 (1:40:57 - 1:45:41): Comprobar si una frase es palíndromo.**
    *   Un palíndromo se lee igual al derecho y al revés, ignorando espacios y mayúsculas/minúsculas (ej: "Ama a la dama").
    *   Solución:
        1.  Pedir la frase.
        2.  Crear una versión sin espacios (como en el ejercicio anterior).
        3.  Crear una versión invertida de la frase sin espacios.
        4.  Comparar la frase sin espacios con su versión invertida usando `equalsIgnoreCase()`.
*   **Ejercicio 15 (1:45:42 - 1:50:49): Juego de adivinar el número.**
    *   Generar un número aleatorio entre 1 y 100.
    *   El usuario tiene 5 intentos para adivinarlo.
    *   Dar pistas ("el número es mayor" o "el número es menor").
    *   Solución: Usar `Random` para el número. Un bucle `while` que se ejecute mientras `!acertado && intentos > 0`. Dentro, pedir número al usuario, comparar, dar pistas y decrementar intentos. Al final, mostrar si ganó o perdió.
*   **Funciones (Métodos) (1:50:50 - 1:55:47):**
    *   Bloques de código reutilizables que realizan una tarea específica.
    *   **Diferencia (coloquial):** "Método" a veces se usa si no devuelve nada (`void`), "función" si devuelve un valor. En Java, ambos son métodos de una clase.
    *   **Declaración:**
        `public static tipoDeRetorno nombreFuncion(tipoParam1 param1, tipoParam2 param2) { // cuerpo ... return valor; // si no es void }`
        *   `public static`: Modificadores (se explicarán más con POO). Por ahora, se usan para funciones dentro de la clase principal que se llaman desde `main`.
        *   `tipoDeRetorno`: El tipo de dato que devuelve la función (`void` si no devuelve nada).
        *   `nombreFuncion`: Nombre descriptivo.
        *   `parametros`: Valores que la función recibe para trabajar. Son opcionales.
        *   `return valor;`: Instrucción para devolver un valor (debe coincidir con `tipoDeRetorno`).
    *   **Llamada a la función:** `nombreFuncion(argumento1, argumento2);`
    *   Ejemplos: `saludar(String nombre)`, `sumar(int a, int b) return a+b;`, `esPar(int num) return num % 2 == 0;`.
*   **Ejercicio 16 (1:55:48 - 1:58:34): Calcular factorial de un número.**
    *   El factorial de N (N!) es `N * (N-1) * ... * 1`.
    *   Solución: Crear una función `factorial(int n)` que use un bucle `for` (de `n-1` hasta 1, o de 1 hasta `n`) para multiplicar los números.
*   **Ejercicio 17 (1:58:35 - 2:00:48): Función para generar número aleatorio en un rango.**
    *   Crear `generaAleatorio(int min, int max)` que devuelva un entero aleatorio entre `min` y `max` (inclusive).
    *   Solución: Usar `Random().nextInt(min, max + 1);` (o la lógica equivalente si `nextInt` con dos args no está disponible).
*   **Ejercicio 18 (2:00:49 - 2:05:40): Generar contraseña aleatoria.**
    *   Crear `generaPassword(int longitud)` que devuelva un String con una contraseña de `longitud` dada, con números, mayúsculas y minúsculas.
    *   Solución:
        *   Usar la función `generaAleatorio` del ejercicio anterior.
        *   En un bucle hasta `longitud`:
            *   Generar un tipo aleatorio (1=número, 2=mayúscula, 3=minúscula).
            *   Según el tipo, generar un carácter aleatorio en el rango ASCII correspondiente (ej: '0'-'9', 'A'-'Z', 'a'-'z').
            *   Castear el número a `char`.
            *   Concatenar al password.
*   **Ejercicio 19 (2:05:41 - 2:12:33): Obtener número de la serie Fibonacci.**
    *   Serie: 1, 1, 2, 3, 5, 8... (cada número es la suma de los dos anteriores).
    *   Crear `serieFibonacci(int posicion)` que devuelva el número en esa `posicion`.
    *   Validar que `posicion >= 1`.
    *   Solución: Usar un bucle. Mantener `num1`, `num2` y `suma`. En cada iteración, `suma = num1 + num2`, luego `num1 = num2` y `num2 = suma`. Manejar los casos base para posición 1 y 2.
*   **Arrays (Arreglos) (2:12:34 - 2:17:40):**
    *   Estructuras para guardar un conjunto de valores **del mismo tipo** bajo un solo nombre.
    *   Tamaño fijo una vez creado.
    *   Acceso a elementos por índice (empezando en 0).
    *   **Creación:**
        *   `tipo[] nombreArray = new tipo[longitud];` (ej: `int[] numeros = new int[5];`)
        *   `tipo[] nombreArray = {valor1, valor2, ...};` (creación e inicialización directa)
    *   **Asignar valor:** `nombreArray[indice] = valor;`
    *   **Obtener valor:** `variable = nombreArray[indice];`
    *   **Obtener longitud:** `nombreArray.length`
    *   **Recorrer (con `for` tradicional):**
        ```java
        for (int i = 0; i < miArray.length; i++) {
            // Usar miArray[i]
        }
        ```
    *   **Recorrer (con `for-each` o "enhanced for loop"):**
        ```java
        for (tipo elemento : miArray) {
            // Usar elemento (es una copia del valor en cada iteración)
        }
        ```
        Más simple para solo leer valores, no permite modificar el array directamente ni acceder al índice.
*   **Ejercicio 20 (2:17:41 - 2:19:56): Suma y media de elementos de un array.**
    *   Crear un array de números. Calcular la suma total y la media.
    *   Solución: Recorrer el array, sumar los elementos. La media es `(double)suma / array.length` (castear para división decimal).
*   **Ejercicio 21 (2:19:57 - 2:22:57): Obtener el mayor y menor de un array.**
    *   Crear un array. Encontrar el elemento mayor y el menor.
    *   Solución: Inicializar `mayor` y `menor` con el primer elemento del array. Luego recorrer desde el segundo elemento, comparando y actualizando `mayor` y `menor` si se encuentra uno más grande/pequeño.
*   **Ejercicio 22 (2:22:58 - 2:26:07): Persona con más edad (usando dos arrays).**
    *   Tener un array de nombres y otro de edades, donde el índice `i` de nombres corresponde al índice `i` de edades.
    *   Indicar el nombre de la persona con más edad.
    *   Solución: Encontrar el índice de la edad mayor. Usar ese índice para obtener el nombre correspondiente.
*   **Clase `Arrays` (Utilidades para Arrays) (2:26:08 - 2:27:50):**
    *   Clase de utilidad con métodos estáticos para trabajar con arrays.
    *   Necesita `import java.util.Arrays;`
    *   `Arrays.toString(miArray)`: Devuelve una representación en String del array (ej: `[1, 2, 3]`). Útil para imprimir.
    *   `Arrays.sort(miArray)`: Ordena el array (modifica el original).
    *   `Arrays.equals(array1, array2)`: Compara si dos arrays tienen el mismo contenido en el mismo orden. (No usar `==` para comparar contenido de arrays).
*   **Ejercicio 23 (2:27:51 - 2:31:31): Comprobar si un array es capicúa.**
    *   Un array es capicúa si se lee igual de izquierda a derecha que de derecha a izquierda (ej: `[1, 2, 3, 2, 1]`).
    *   Solución: Crear una copia invertida del array. Comparar el original con el invertido usando `Arrays.equals()`.
*   **Ejercicio 24 (2:31:32 - 2:34:53): Fusionar dos arrays en uno.**
    *   Crear dos arrays. Crear un tercer array que contenga todos los elementos de los dos primeros.
    *   Solución: El tercer array tendrá longitud `array1.length + array2.length`. Copiar elementos de `array1` al inicio de `array3`. Luego copiar elementos de `array2` a continuación en `array3`.
*   **Arrays y Funciones (Paso por Valor vs. Paso por Referencia) (2:34:54 - 2:37:21):**
    *   **Tipos Primitivos (int, double, etc.):** Se pasan a las funciones **por valor**. La función recibe una copia. Si la función modifica el parámetro, el valor original fuera de la función no cambia.
    *   **Objetos (incluidos Arrays):** Se pasan a las funciones **por referencia** (técnicamente, la referencia se pasa por valor, pero apunta al mismo objeto en memoria). Si la función modifica el contenido del objeto (ej: los elementos de un array), los cambios son visibles fuera de la función porque se está operando sobre el mismo objeto.
    *   No es necesario que una función devuelva un array si solo lo modifica; los cambios ya estarán hechos en el array original.
*   **Ejercicio 25 (2:37:22 - 2:40:46): Indicar si un elemento existe en un array (usando función).**
    *   Crear `existeElemento(int[] array, int elemento)` que devuelva `true` si `elemento` está en `array`, `false` si no.
    *   Solución: Recorrer el array. Si se encuentra el elemento, `return true;`. Si el bucle termina sin encontrarlo, `return false;` (fuera del bucle).
*   **Ejercicio 26 (2:40:47 - 2:43:49): Rellenar array con números aleatorios (usando función).**
    *   Crear `rellenarArrayAleatorios(int[] array, int min, int max)` que modifique `array` llenándolo con números aleatorios entre `min` y `max`.
    *   Reutilizar la función `generaAleatorio` de un ejercicio anterior.
*   **Matrices (Arrays Bidimensionales) (2:43:50 - 2:47:29):**
    *   Arrays de arrays. Se pueden ver como tablas con filas y columnas.
    *   **Creación:**
        *   `tipo[][] nombreMatriz = new tipo[numFilas][numColumnas];`
        *   `tipo[][] nombreMatriz = {{f0c0,f0c1},{f1c0,f1c1},...};` (inicialización directa)
    *   **Acceso:** `nombreMatriz[fila][columna]` (ambos índices empiezan en 0).
    *   **Longitud:**
        *   `nombreMatriz.length`: Número de filas.
        *   `nombreMatriz[fila].length`: Número de columnas en esa `fila` (pueden ser irregulares, "jagged arrays", aunque comúnmente son regulares).
    *   **Recorrer (con bucles `for` anidados):**
        ```java
        for (int i = 0; i < matriz.length; i++) { // Recorre filas
            for (int j = 0; j < matriz[i].length; j++) { // Recorre columnas de la fila i
                // Usar matriz[i][j]
            }
        }
        ```
*   **Ejercicio 27 (2:47:30 - 2:50:58): Sumar valores de una fila de una matriz.**
    *   Dada una matriz y un número de fila, sumar los elementos de esa fila.
    *   Usar `Math.clamp()` para asegurar que el índice de fila pedido sea válido.
*   **Ejercicio 28 (2:50:59 - 2:54:05): Sumar valores de una columna de una matriz.**
    *   Similar al anterior, pero sumar los elementos de una columna específica.
*   **Ejercicio 29 (2:54:06 - 3:03:28): Mover una 'X' en un tablero (matriz).**
    *   Crear una matriz de caracteres (tablero) con '.' y una 'X'.
    *   Permitir al usuario mover la 'X' (arriba, abajo, izquierda, derecha) sin salirse del tablero.
    *   Solución: Mantener la posición (fila, columna) de la 'X'. En un bucle `while`, mostrar el tablero, pedir dirección. Antes de mover, verificar límites. Si es válido, "limpiar" la posición actual de la 'X' (poner '.'), actualizar fila/columna, y poner 'X' en la nueva posición.
*   **Excepciones (Manejo de Errores) (3:03:29 - 3:09:36):**
    *   Eventos anómalos que ocurren durante la ejecución y pueden interrumpir el flujo normal del programa.
    *   Ejemplos: `ArithmeticException` (división por cero), `InputMismatchException` (Scanner espera un número y recibe texto), `ArrayIndexOutOfBoundsException` (acceder a un índice de array inválido).
    *   **Bloque `try-catch`:**
        ```java
        try {
            // Código que podría lanzar una excepción
        } catch (TipoDeException1 e1) {
            // Código para manejar la excepción TipoDeException1
        } catch (TipoDeException2 e2) {
            // Código para manejar la excepción TipoDeException2
        } finally { // Opcional
            // Código que se ejecuta siempre, haya o no excepción
        }
        ```
    *   Si ocurre una excepción en el bloque `try`, se salta al bloque `catch` correspondiente. Si no hay `catch` adecuado, el programa termina.
    *   `Exception` es la clase padre de muchas excepciones. Se puede usar `catch (Exception e)` para capturar casi cualquier excepción, pero es mejor ser específico.
    *   **`e.getMessage()`:** Obtiene un mensaje descriptivo de la excepción.
    *   **`Scanner` y `InputMismatchException`:** Si ocurre, es bueno llamar a `sn.next()` dentro del `catch` para "consumir" la entrada incorrecta y evitar bucles infinitos si se vuelve a pedir entrada.
    *   **Lanzar Excepciones Personalizadas (`throw new ExceptionType("mensaje");`):**
        Se puede crear y lanzar una excepción si una condición de negocio no se cumple.
    *   **Cláusula `throws` en la firma del método:**
        `public void miMetodo() throws MiException { ... }`
        Indica que `miMetodo` puede lanzar `MiException` (una "checked exception") y quien lo llame debe manejarla (con `try-catch`) o declararla también con `throws`.
    *   **Multicatch:** Se pueden tener varios `catch` para diferentes tipos de excepciones. Se evalúan en orden. El más general (`Exception`) debería ir al final.
*   **Enumerados (`enum`) (3:09:37 - 3:12:38):**
    *   Tipo de dato especial que permite definir un conjunto de constantes con nombre.
    *   Ejemplo: `enum Color { ROJO, VERDE, AZUL }`
    *   **Creación en NetBeans:** Clic derecho en el paquete > `New > Java Enum`.
    *   **Uso:**
        *   `Color miColor = Color.ROJO;`
        *   `Color.values()`: Devuelve un array con todas las constantes del enum.
        *   `Color.valueOf("NOMBRE_CONSTANTE")`: Convierte un String al valor enum correspondiente (lanza `IllegalArgumentException` si el String no coincide).
    *   Útil para limitar los valores posibles de una variable, en lugar de usar Strings "mágicos".
*   **Ejercicio 30 (3:12:39 - 3:21:12): Días de un mes usando enumerado.**
    *   Crear un `enum Meses { ENERO, FEBRERO, ..., DICIEMBRE }`.
    *   Pedir al usuario un mes (String).
    *   Convertir el String a un valor del `enum Meses` (usando `try-catch` para `IllegalArgumentException`).
    *   Usar un `switch` sobre el valor del `enum` para determinar el número de días.
    *   Para febrero, pedir el año y usar la función `esBisiesto` para determinar si tiene 28 o 29 días.
    *   Manejar `InputMismatchException` si se introduce texto en lugar de año.

---

**Parte 12: Despedida (3:21:13 - Final)**

*   Agradecimientos y recordatorio de que el código está en GitHub.
*   Anuncio de futuros cursos (Programación Orientada a Objetos, ficheros, aplicaciones gráficas, lambdas, etc.).
*   Petición de "like" y suscripción.

---

Este resumen detallado cubre todos los puntos clave, conceptos y ejemplos del video, proporcionando una guía completa para el aprendizaje. ¡Espero que te sea de gran ayuda!
