# **Java How to Program, Early Objects (11th ed.)**

## *Java Desde el Objeto: Un Enfoque Integral* / *Dominando la Programación Orientada a Objetos desde el Principio con la Metodología Deitel*

---

## **Resumen General (Abstract)**

Esta undécima edición de *Java How to Program* [1] adopta un enfoque pedagógico **"Early Objects"**, introduciendo los conceptos fundamentales y el paradigma de la programación orientada a objetos (POO) – clases, objetos, encapsulación, herencia y polimorfismo – desde las etapas más tempranas del proceso de aprendizaje de Java. Aborda directamente la necesidad de formar programadores que **piensen en términos de objetos desde el principio**, una habilidad considerada crucial para el desarrollo eficaz de software moderno, especialmente en el ecosistema Java donde la OOP es central. Utilizando el distintivo y probado enfoque **"Live-Code"** de Deitel, el libro presenta la teoría a través de **ejemplos de código Java completos, funcionales y meticulosamente comentados**, seguidos de explicaciones detalladas y salidas de muestra para ilustrar los conceptos en acción. Cubre de manera exhaustiva no solo los fundamentos del lenguaje Java (tipos de datos primitivos, estructuras de control, métodos, arrays) sino también la POO avanzada, manejo robusto de excepciones, entrada/salida de archivos (E/S), genéricos, el framework de Colecciones de Java, estructuras de datos fundamentales, concurrencia básica y desarrollo de interfaces gráficas de usuario (GUI) utilizando JavaFX. Su contribución principal es ofrecer una **introducción rigurosa, masiva y completa** a Java que prioriza e integra la comprensión profunda del paradigma orientado a objetos como el núcleo central desde el comienzo del viaje de aprendizaje.

---

## **Prefacio Contextual**

En el panorama de la enseñanza de la programación introductoria, existe un debate pedagógico continuo sobre el momento óptimo para introducir los conceptos de la Programación Orientada a Objetos. El enfoque "Early Objects" adoptado por este libro [1] responde a la perspectiva de que **integrar la POO desde el principio** ayuda a los estudiantes a desarrollar un modelo mental más coherente y alineado con las prácticas predominantes en la industria del desarrollo de software, donde Java se utiliza casi exclusivamente dentro de un paradigma orientado a objetos. Publicado en 2018, este texto es altamente relevante para cursos universitarios (típicamente secuencias CS1/CS2) y programas de formación profesional que adoptan explícitamente esta filosofía pedagógica "objects-first". Viene a llenar la necesidad de un **texto exhaustivo, probado a lo largo de múltiples ediciones, y extremadamente rico en ejemplos** que guíe a los estudiantes a través de la considerable complejidad del lenguaje Java y el paradigma OOP de una manera estructurada y detallada, utilizando el lenguaje estándar de la industria para una amplia gama de aplicaciones empresariales y de sistemas.

---

## **Objetivos de Aprendizaje**

Al completar la lectura y estudio activo de este libro, el lector podrá:

1.  **Comprender y aplicar con solidez** los principios fundamentales de la programación orientada a objetos (Clases, Objetos, Encapsulación, Herencia, Polimorfismo) en el diseño e implementación de programas Java.
2.  **Dominar la sintaxis y la semántica** del lenguaje Java, incluyendo el uso correcto de tipos de datos primitivos, operadores, estructuras de control (selección, repetición) y métodos.
3.  **Diseñar e implementar clases Java robustas** y bien encapsuladas, gestionando eficazmente el estado (atributos) y el comportamiento (métodos) de los objetos.
4.  **Manejar excepciones** de forma efectiva para crear aplicaciones Java más fiables y resistentes a errores en tiempo de ejecución.
5.  **Utilizar eficazmente el framework de Colecciones de Java** (Listas, Sets, Maps) y los genéricos para gestionar grupos de objetos de manera flexible y segura en cuanto a tipos.
6.  **Comprender e implementar los conceptos básicos de la concurrencia** en Java (hilos) y realizar operaciones fundamentales de entrada/salida de archivos.
7.  **Desarrollar interfaces gráficas de usuario (GUI)** interactivas utilizando la biblioteca JavaFX.

---

## **Audiencia Objetivo**

Este libro está dirigido principalmente a:

*   **Estudiantes universitarios** en cursos introductorios e intermedios de programación Java (CS1 y CS2) que siguen un currículo con enfoque **"Early Objects"**.
*   **Principiantes en programación** (aunque puede ser denso) que desean una introducción **muy completa, detallada y rigurosa** a Java, con un énfasis temprano en la POO.
*   **Desarrolladores con experiencia en otros lenguajes** que buscan aprender Java en profundidad y desde una perspectiva orientada a objetos desde el inicio.
*   **Educadores** que buscan un texto exhaustivo, con abundantes ejemplos de código "Live-Code" y materiales de apoyo para cursos de Java que adopten el enfoque "Early Objects".

**Conocimiento Previo Recomendado**: **Formalmente ninguno**, ya que pretende ser un libro introductorio. Sin embargo, dada su **extensión, densidad y ritmo rápido** en la introducción de conceptos (incluyendo OOP temprana), una **aptitud para el pensamiento lógico y abstracto**, y preferiblemente alguna **experiencia previa muy básica con la programación** o al menos con la resolución de problemas estructurados, resultará **muy beneficiosa**. Puede ser un libro desafiante como primer contacto absoluto con la programación.

---

## **Estructura y Organización**

La característica definitoria de este libro es su estructura **"Early Objects"**. La organización está diseñada para sumergir al estudiante en el paradigma orientado a objetos casi desde el principio:

1.  **Introducción Fundamental (Caps. 1-2)**: Comienza con una introducción a las computadoras, Java y el entorno de desarrollo. Rápidamente, en el capítulo 2 o 3, introduce el concepto de **clases y objetos** utilizando ejemplos simples (ej. una clase `Account` o `GradeBook`), mostrando cómo crear objetos y llamar a sus métodos. Esto ocurre *antes* de una cobertura exhaustiva de todas las estructuras de control.
2.  **Control de Flujo (Caps. 3-4 aprox.)**: Aunque se introducen objetos temprano, se dedican capítulos a cubrir formalmente las estructuras de control: selección (`if`, `else`, `switch`) y repetición (`while`, `for`, `do-while`). Los ejemplos pueden seguir utilizando los objetos introducidos.
3.  **Métodos (Cap. 5 aprox.)**: Profundiza en la definición y uso de métodos, paso de argumentos, sobrecarga de métodos y alcance de variables.
4.  **Arrays y ArrayLists (Cap. 6 aprox.)**: Introduce las estructuras de datos básicas para colecciones: arrays primitivos y la clase `ArrayList` del framework de Colecciones.
5.  **Profundización en Clases y Objetos (Caps. 7-8 aprox.)**: Vuelve a la OOP con más detalle, cubriendo temas como miembros `static`, `final`, composición ("has-a"), enumeraciones (`enum`), recolección de basura.
6.  **OOP Avanzada (Caps. 9-10 aprox.)**: Cubre los pilares más avanzados de la OOP: **Herencia** (subclases, superclases, `protected`, override) y **Polimorfismo** (variables de superclase referenciando objetos de subclase, métodos abstractos, clases abstractas, interfaces).
7.  **Temas Esenciales Adicionales (Caps. 11+)**:
    *   **Manejo de Excepciones**: `try`, `catch`, `finally`, jerarquía de excepciones.
    *   **GUI con JavaFX**: Componentes gráficos, layouts, manejo de eventos.
    *   **Strings y Caracteres**: Manipulación avanzada de texto.
    *   **Archivos, Streams y Serialización de Objetos**: E/S de archivos de texto y binarios, `ObjectInputStream`/`ObjectOutputStream`.
    *   **Genéricos**: Programación con tipos parametrizados.
    *   **Colecciones**: Uso detallado de `List`, `Set`, `Map` y sus implementaciones.
    *   **Estructuras de Datos**: Implementación de listas enlazadas, pilas, colas, árboles (nivel CS2).
    *   **Concurrencia**: Introducción a hilos (`Thread`, `Runnable`), sincronización básica.
    *   **(Posiblemente otros)**: Networking básico, JDBC para bases de datos, etc.

La **lógica organizativa** es introducir la idea fundamental de **objetos como bloques de construcción** muy temprano, para que el estudiante piense en términos de entidades con estado y comportamiento desde el inicio. Luego, se cubren las herramientas de control y estructuración (bucles, métodos, arrays) necesarias para trabajar con esos objetos, para finalmente profundizar en los aspectos más sofisticados de OOP y temas avanzados de Java y CS.

---

## **Análisis por Capítulo (Estimado y Resumido)**

*Nota: Los libros Deitel son muy extensos (20+ capítulos a menudo). Se presenta una estructura representativa.*

---

### **Capítulo 1: Introducción a Computadoras, Internet y Java**

*   **Resumen**: Contexto computacional, hardware/software, lenguajes, historia de Java, JVM, proceso de desarrollo Java (compilar/ejecutar), configuración entorno (JDK, IDE). Primer programa `HelloWorld`.
*   **Objetivos**: Entender contexto; Configurar entorno; Escribir/ejecutar programa Java básico.
*   **Contexto**: Base conceptual y práctica inicial.
*   **Conceptos**: Hardware, Software, Java, JVM, Bytecode, JDK, IDE, `public static void main`.
*   **Referencia IEEE**: [1] P. Deitel and H. Deitel, "Cap. 1...," *Java How to Program, Early Objects*, 11th ed. Pearson, 2018.

### **Capítulo 2: Introducción a Aplicaciones Java: Entrada/Salida y Operadores**

*   **Resumen**: Tipos primitivos (`int`, `double`, `char`, `boolean`), variables, asignación, operadores aritméticos, entrada (usando `Scanner`), salida (`System.out.print`/`println`/`printf`).
*   **Objetivos**: Usar tipos/variables; Realizar aritmética; Leer entrada; Mostrar salida formateada.
*   **Contexto**: Manipulación de datos básicos e interacción simple.
*   **Conceptos**: Tipos Primitivos, Variables, Operadores Aritméticos, `Scanner`, `System.out`, `printf`.
*   **Referencia IEEE**: [2] P. Deitel and H. Deitel, "Cap. 2...," *Java How to Program, Early Objects*, 11th ed.

### **Capítulo 3: Introducción a Clases, Objetos, Métodos y Strings**

*   **Resumen**: **Introducción temprana a OOP**. Definición de clases simples (ej. `Account`), atributos (variables de instancia), métodos (comportamiento), creación de objetos (`new`), llamada a métodos. Uso básico de la clase `String`.
*   **Objetivos**: Entender clase/objeto; Definir clase simple; Crear/usar objetos; Llamar métodos; Usar `String` básico.
*   **Contexto**: Introduce el paradigma central del libro ("Early Objects").
*   **Conceptos**: Clases, Objetos, Instancia, Atributos, Métodos, `new`, `String`.
*   **Referencia IEEE**: [3] P. Deitel and H. Deitel, "Cap. 3...," *Java How to Program, Early Objects*, 11th ed.

### **Capítulo 4: Estructuras de Control I: Selección**

*   **Resumen**: Sentencias `if`, `if-else`, `if-else if-else`, operadores de comparación/lógicos, operador ternario (`? :`), sentencia `switch`.
*   **Objetivos**: Implementar lógica condicional; Usar operadores booleanos; Aplicar `switch`.
*   **Contexto**: Toma de decisiones en programas (a menudo aplicado a objetos).
*   **Conceptos**: `if`, `else`, `switch`, Operadores (Comparación, Lógicos), Ternario.
*   **Referencia IEEE**: [4] P. Deitel and H. Deitel, "Cap. 4...," *Java How to Program, Early Objects*, 11th ed.

### **Capítulo 5: Estructuras de Control II: Repetición**

*   **Resumen**: Bucles `while`, `for`, `do-while`. Control por contador/centinela. Sentencias `break`/`continue`.
*   **Objetivos**: Implementar diferentes tipos de bucles; Usar `break`/`continue`; Resolver problemas con repetición.
*   **Contexto**: Ejecución repetitiva (a menudo sobre colecciones de objetos o para simulación).
*   **Conceptos**: `while`, `for`, `do-while`, `break`, `continue`, Bucles Anidados.
*   **Referencia IEEE**: [5] P. Deitel and H. Deitel, "Cap. 5...," *Java How to Program, Early Objects*, 11th ed.

### **Capítulo 6: Métodos: Una Mirada más Profunda**

*   **Resumen**: Argumentos/parámetros, paso por valor (primitivos vs referencias a objetos), sobrecarga de métodos, alcance, recursión (introducción), métodos `static`.
*   **Objetivos**: Definir/llamar métodos complejos; Entender paso de args; Sobrecargar métodos; Entender alcance/`static`; Intro a recursión.
*   **Contexto**: Profundiza en la modularidad y el comportamiento de los objetos.
*   **Conceptos**: Métodos, Argumentos, Parámetros, Paso por Valor/Referencia (conceptual), Sobrecarga, Alcance, `static`, Recursión (intro).
*   **Referencia IEEE**: [6] P. Deitel and H. Deitel, "Cap. 6...," *Java How to Program, Early Objects*, 11th ed.

### **Capítulo 7: Arrays y ArrayLists**

*   **Resumen**: Arrays unidimensionales/multidimensionales. Declaración, creación, inicialización, acceso, paso a métodos. Introducción a `ArrayList` (colección dinámica). Bucles `for` mejorados.
*   **Objetivos**: Usar arrays (fijos); Usar `ArrayList` (dinámico); Procesar colecciones con bucles.
*   **Contexto**: Estructuras de datos para almacenar colecciones.
*   **Conceptos**: Arrays, `ArrayList`, Índice, Tamaño Fijo vs Dinámico, Bucles For Mejorados.
*   **Referencia IEEE**: [7] P. Deitel and H. Deitel, "Cap. 7...," *Java How to Program, Early Objects*, 11th ed.

### **Capítulo 8: Clases y Objetos: Una Mirada más Profunda**

*   **Resumen**: Composición ("has-a"), `this`, `static` (miembros/métodos), `final`, `enum`, recolección de basura (conceptual), paquetes (`import`).
*   **Objetivos**: Implementar composición; Usar `this`; Entender `static`/`final`/`enum`; Comprender paquetes.
*   **Contexto**: Detalles y técnicas adicionales para diseño de clases robusto.
*   **Conceptos**: Composición, `this`, `static`, `final`, `enum`, Paquetes, `import`, Garbage Collection.
*   **Referencia IEEE**: [8] P. Deitel and H. Deitel, "Cap. 8...," *Java How to Program, Early Objects*, 11th ed.

### **Capítulo 9: Programación Orientada a Objetos: Herencia**

*   **Resumen**: Concepto de herencia, superclases, subclases, `extends`, `protected`, override de métodos, `super`, constructores en herencia, jerarquía `Object`.
*   **Objetivos**: Implementar herencia; Usar `protected`/`super`; Sobrescribir métodos; Entender jerarquía `Object`.
*   **Contexto**: Pilar fundamental de OOP para reutilización y especialización.
*   **Conceptos**: Herencia, Superclase, Subclase, `extends`, `protected`, Override, `super`, `Object`.
*   **Referencia IEEE**: [9] P. Deitel and H. Deitel, "Cap. 9...," *Java How to Program, Early Objects*, 11th ed.

### **Capítulo 10: Programación Orientada a Objetos: Polimorfismo e Interfaces**

*   **Resumen**: Polimorfismo, clases/métodos abstractos (`abstract`), interfaces (`interface`), polimorfismo con interfaces. Casting de objetos.
*   **Objetivos**: Entender/aplicar polimorfismo; Usar clases/métodos abstractos; Definir/implementar interfaces.
*   **Contexto**: Pilar de OOP para flexibilidad y diseño desacoplado.
*   **Conceptos**: Polimorfismo, Clases Abstractas, Métodos Abstractos, Interfaces, `implements`.
*   **Referencia IEEE**: [10] P. Deitel and H. Deitel, "Cap. 10...," *Java How to Program, Early Objects*, 11th ed.

### **Capítulo 11: Manejo de Excepciones: Una Mirada más Profunda**

*   **Resumen**: Bloques `try-catch-finally`, jerarquía de excepciones (`Throwable`, `Exception`, `RuntimeException`), excepciones checked vs unchecked, `throw`, `throws`, creación de excepciones personalizadas.
*   **Objetivos**: Manejar excepciones robustamente; Entender jerarquía/tipos; Lanzar excepciones.
*   **Contexto**: Programación defensiva y manejo de errores.
*   **Conceptos**: Excepciones, `try`, `catch`, `finally`, `throw`, `throws`, Checked/Unchecked Exceptions.
*   **Referencia IEEE**: [11] P. Deitel and H. Deitel, "Cap. 11...," *Java How to Program, Early Objects*, 11th ed.

### **Capítulo 12: GUI con JavaFX (Parte 1)**

*   **Resumen**: Introducción a JavaFX: Stage, Scene, nodos, controles básicos (Label, Button, TextField), layouts (ej. FlowPane, BorderPane), manejo de eventos simple (action events).
*   **Objetivos**: Crear ventana JavaFX; Usar controles/layouts básicos; Manejar eventos de botón.
*   **Contexto**: Desarrollo de interfaces gráficas de usuario en Java moderno.
*   **Conceptos**: JavaFX, Stage, Scene, Node, Controls, Layouts, Event Handling.
*   **Referencia IEEE**: [12] P. Deitel and H. Deitel, "Cap. 12...," *Java How to Program, Early Objects*, 11th ed.

*(Se omiten resúmenes detallados de capítulos posteriores sobre Strings, Archivos, Genéricos, Colecciones, DS, Concurrencia, etc., por brevedad, pero seguirían el mismo patrón de detalle y enfoque práctico Deitel).*

---

## **Estrategia de Lectura Recomendada**

1.  **Secuencia Óptima**: **Mayormente lineal**. El enfoque "Early Objects" introduce clases temprano (Cap 3), pero luego sigue una progresión bastante estándar: control, métodos, arrays, OOP avanzada, temas adicionales. Es crucial seguir el orden, especialmente al principio. Capítulos sobre temas avanzados (GUI, Colecciones, Concurrencia) pueden tener cierta flexibilidad una vez dominados los fundamentos y OOP.
2.  **Niveles de Lectura**:
    *   **Familiarización Rápida**: Ojear la tabla de contenidos, introducciones/resúmenes de capítulo, y especialmente los ejemplos "Live-Code" completos. Ayuda a captar la inmensa cobertura y el estilo (10-15 horas). *No sirve para aprender*.
    *   **Lectura Profunda (Método Previsto)**: Leer cada capítulo **meticulosamente**. **Escribir, compilar, ejecutar y depurar (entender)** cada ejemplo "Live-Code". **Resolver una gran cantidad de ejercicios** de final de capítulo (autoevaluación, programación, "Making a Difference"). Este libro exige un estudio muy activo y detallado (Estimado: 150-250+ horas).
    *   **Lectura Selectiva (Referencia)**: Dada su exhaustividad, puede servir como referencia detallada sobre temas específicos de Java o CS una vez completado. El índice es fundamental.
3.  **Tiempos Estimados**:
    *   **Por Capítulo**: Extremadamente variable dada la densidad. Capítulos fundamentales pueden requerir 8-15 horas. Capítulos sobre OOP avanzada, GUI, Colecciones, DS o Concurrencia pueden necesitar 15-25+ horas cada uno, incluyendo la práctica intensa.
    *   **Libro Completo**: Es un libro diseñado para **dos semestres** universitarios (CS1+CS2). Para un autodidacta, dominarlo completamente requiere una inversión masiva de tiempo: **150 a 250 horas o más**, distribuidas en varios meses.
4.  **Puntos de Conexión**:
    *   **Cap. 3 (Objetos) -> Caps. 4-7 (Control, Métodos, Arrays)**: Constantemente aplicar las estructuras y técnicas aprendidas a los objetos introducidos tempranamente.
    *   **Caps. 9-10 (OOP Avanzada)**: Conectar cómo la herencia y el polimorfismo extienden y flexibilizan las clases definidas en capítulos anteriores (3, 8).
    *   **Cap. 7 (Arrays/ArrayLists) -> Caps. de Colecciones/DS**: Ver cómo el framework de Colecciones y las estructuras de datos personalizadas ofrecen alternativas más potentes a los arrays básicos.
    *   **Cap. 11 (Excepciones)**: Aplicar el manejo de excepciones en todo el código posterior, especialmente en E/S (Archivos) y GUI.
5.  **Actividades Complementarias**:
    *   **¡HACER LOS EJERCICIOS!**: Absolutamente crucial en un libro Deitel. Son numerosos y variados, y la clave para la maestría.
    *   **Usar un IDE y Debugger**: Compilar, ejecutar y, sobre todo, depurar el código (seguir paso a paso, inspeccionar variables) es esencial para entender la ejecución.
    *   **Leer el Código Detalladamente**: Presta atención a los comentarios y al estilo del código "Live-Code".
    *   **Proyectos Pequeños/Medianos**: Intentar aplicar los conceptos en proyectos un poco más grandes que los ejercicios (ej. una simulación simple, una aplicación CRUD básica con GUI después de cubrir esos temas).
    *   **Documentación de Java API**: Consultar la documentación oficial de las clases de la biblioteca estándar (Scanner, ArrayList, String, etc.) para profundizar.

---

## **Lecturas Complementarias Recomendadas**

1.  **Fundamentos Previos (Si el ritmo "Early Objects" es difícil)**:
    *   [15] P. Deitel and H. Deitel, *Java How to Program, Late Objects*, 11th ed. Pearson, 2018.
        *   *Justificación*: La versión "Late Objects" del mismo libro. Cubre los fundamentos procedimentales *antes* de introducir OOP. Podría ser una alternativa si el enfoque "Early Objects" resulta confuso al principio.
        *   *Relación*: Misma cobertura final, diferente secuencia pedagógica inicial.
    *   [16] T. Gaddis, *Starting Out with Java: From Control Structures through Objects*, 6th ed. Pearson, 2016.
        *   *Justificación*: Introducción mucho más gradual y paso a paso, estilo "Late Objects", si Deitel resulta demasiado denso o rápido.
        *   *Relación*: Cubre los fundamentos (hasta OOP básica) a un ritmo más lento.

2.  **Profundización Teórica (Java Core / Diseño)**:
    *   [17] J. Bloch, *Effective Java*, 3rd ed. Addison-Wesley, 2018.
        *   *Justificación*: **Esencial** para cualquier desarrollador Java serio *después* de aprender los fundamentos. Colección de "items" con mejores prácticas para escribir código Java excelente.
        *   *Relación*: Profundiza en cómo usar bien las características de Java cubiertas por Deitel (OOP, genéricos, excepciones, etc.).
    *   [18] K. Sierra and B. Bates, *Head First Java*, 3rd ed. O'Reilly Media, 2022.
        *   *Justificación*: Enfoque visual y cognitivo (Head First) para aprender Java, puede ser un buen complemento si el estilo Deitel es muy formal. Cubre fundamentos y OOP.
        *   *Relación*: Pedagogía alternativa para los mismos temas centrales.

3.  **Aplicaciones Prácticas (Frameworks / Dominios)**:
    *   [19] C. S. Horstmann, *Core Java Volume I--Fundamentals*, 12th ed. Prentice Hall, 2021. (Y Volumen II - Advanced Features).
        *   *Justificación*: Referencia muy respetada y detallada sobre Java SE, a menudo vista como un paso intermedio/avanzado después de Deitel. Cubre temas prácticos y de la biblioteca estándar en profundidad.
        *   *Relación*: Profundización en Java SE.
    *   [20] Pluralsight Paths sobre Spring Framework (ej. Refs [9-13] de la lista Java original).
        *   *Justificación*: Si el objetivo es el desarrollo backend/enterprise con Java, Spring es el framework dominante. Estas rutas cubren cómo usarlo.
        *   *Relación*: Aplicación práctica de Java en el ecosistema empresarial moderno.
    *   [21] Libros sobre Android Development (si el interés es móvil).
        *   *Justificación*: Java (y Kotlin) son lenguajes clave para el desarrollo Android nativo.
        *   *Relación*: Aplicación de Java a un dominio específico (móvil).

4.  **Perspectivas Alternativas (Otros Textos CS1/CS2)**:
    *   [22] Y. D. Liang, *Introduction to Java Programming and Data Structures*, Comp. Ver., 11th ed. Pearson, 2019.
        *   *Justificación*: Competidor directo de Deitel, también muy completo y riguroso, con un fuerte enfoque en resolución de problemas y cobertura integrada de DS&A.
        *   *Relación*: Alternativa principal con enfoque similar ("fundamentals-first", aunque no necesariamente "early objects").

5.  **Desarrollos Recientes (Java SE > 11)**:
    *   [23] Documentación Oficial de Java SE (Oracle / OpenJDK - ej. https://docs.oracle.com/en/java/javase/17/docs/api/index.html para Java 17).
        *   *Justificación*: Fuente autorizada para las APIs de Java y las características de versiones posteriores a la cubierta por el libro (ej. Records, Sealed Classes, Pattern Matching introducidos después de Java 11).
        *   *Relación*: Referencia esencial y actualización del lenguaje.
    *   [24] Blogs y artículos sobre nuevas características de Java (ej. Baeldung, Oracle Java Magazine, InfoQ).
        *   *Justificación*: Para mantenerse al día con la rápida evolución de Java post-Java 8/11.
        *   *Relación*: Información sobre características no cubiertas en la 11ª edición (2018).

---

## **Formato y Estilo**

Esta introducción se ha generado utilizando Markdown con la intención de cumplir con los requisitos de formato y estilo:

*   Uso consistente de encabezados (`#`, `##`, `###`) para la jerarquía.
*   Uso de **negritas**, *cursivas* y `código` para énfasis y claridad.
*   Listas (numeradas y con viñetas) para organizar la información.
*   Espaciado adecuado para mejorar la legibilidad visual.
*   Referencias en formato IEEE como se solicitó.
*   Inclusión del título original y la propuesta de título en español latino.

## **Ejemplo de Referencia IEEE (Aplicado)**

[1] P. Deitel and H. Deitel, "Capítulo 1: Introducción a Computadoras, Internet y Java," en *Java How to Program, Early Objects*, 11th ed. Upper Saddle River, NJ, USA: Pearson, 2018, pp. 1-XX (estimado).

---

