# **Practical Python Data Wrangling and Data Quality: Getting Started with Reading, Cleaning, and Analyzing Data**

## *Domando Datos con Python: Guía Práctica de Wrangling y Calidad* / *Técnicas Esenciales para Leer, Limpiar, Transformar y Asegurar la Fiabilidad de tus Datos*

---

## **Resumen General (Abstract)**

Este libro [1] se enfoca de manera específica y práctica en las etapas cruciales, a menudo subestimadas pero fundamentales, del ***data wrangling*** (el proceso de adquisición, limpieza y transformación de datos) y la **garantía de la calidad de los datos** utilizando el lenguaje de programación Python. Aborda frontalmente el problema omnipresente y consumidor de tiempo de que los datos del mundo real rara vez están listos para el análisis o la modelización, siendo inherentemente "sucios", inconsistentes o incompletos. El enfoque es eminentemente **práctico y orientado a tareas**, guiando sistemáticamente al lector a través del proceso completo: adquisición de datos de diversas fuentes (archivos planos, bases de datos, APIs web), inspección detallada y perfilado para identificar problemas, aplicación de técnicas rigurosas de limpieza (manejo de valores faltantes, corrección de inconsistencias, tratamiento de valores atípicos, validación de tipos) y transformación de datos para adecuarlos a las necesidades del análisis. Utiliza extensivamente bibliotecas estándar de Python y herramientas populares del ecosistema de datos como Pandas y NumPy para ilustrar las técnicas. Su contribución principal y distintiva es ofrecer una **guía dedicada, detallada y metodológica** sobre las mejores prácticas y los métodos efectivos para convertir datos crudos y desordenados en conjuntos de datos fiables, consistentes y listos para generar insights válidos o entrenar modelos precisos, haciendo hincapié constante en la **importancia fundamental de la calidad de los datos** bajo el principio de "garbage in, garbage out".

---

## **Prefacio Contextual**

Mientras que una gran cantidad de recursos educativos en ciencia de datos y machine learning se centran en las fases de modelado, evaluación o visualización, este libro [1] llena una brecha crítica y persistente al abordar en profundidad la fase que, según múltiples estudios y la experiencia práctica, consume la mayor parte del tiempo y esfuerzo en la mayoría de los proyectos de datos: la **preparación y limpieza de datos**. Surge en un contexto tecnológico donde la conciencia sobre el impacto directo de la calidad de los datos en la fiabilidad de los análisis y la precisión de los modelos de IA ("garbage in, garbage out") es cada vez mayor y más explícita. Es particularmente relevante para cualquier profesional de datos (analista, científico, ingeniero) que se enfrente a la realidad cotidiana de trabajar con datos imperfectos, heterogéneos y provenientes de múltiples fuentes, y que necesite un conjunto de **herramientas conceptuales y técnicas sistemáticas** para abordarlos eficazmente. Se diferencia claramente de textos más generales de análisis de datos al profundizar específicamente en las técnicas, desafíos y flujos de trabajo del *data wrangling* y la validación, proveyendo un manual práctico para esta disciplina esencial pero a menudo descuidada.

---

## **Objetivos de Aprendizaje**

Al completar la lectura y la práctica de los ejemplos de este libro, el lector podrá:

1.  **Leer y adquirir datos** de una variedad de formatos y fuentes comunes, incluyendo archivos planos (CSV, Excel, JSON), bases de datos SQL y APIs web, utilizando bibliotecas Python apropiadas.
2.  **Inspeccionar y perfilar conjuntos de datos** de manera sistemática para identificar problemas estructurales y de calidad, como valores faltantes, tipos de datos incorrectos, inconsistencias y valores atípicos.
3.  **Aplicar un repertorio de técnicas** estándar y robustas para limpiar datos utilizando Pandas, incluyendo diferentes estrategias para manejar valores faltantes, corregir inconsistencias lógicas y de formato, y detectar/tratar valores atípicos.
4.  **Transformar y remodelar datos** para adecuarlos a las necesidades específicas del análisis o modelado posterior (ej., cambio de tipos, creación de nuevas variables a partir de existentes, normalización/escalado básico, pivotaje).
5.  **Implementar controles de validación de datos** programáticamente para asegurar la integridad, coherencia y cumplimiento de reglas de negocio en los conjuntos de datos procesados.
6.  **Utilizar eficazmente las funcionalidades de Pandas** y otras bibliotecas relevantes de Python diseñadas específicamente para las tareas de data wrangling y aseguramiento de calidad.
7.  **Comprender y aplicar un flujo de trabajo estructurado** y reproducible para la preparación de datos, desde la adquisición hasta la validación final.

---

## **Audiencia Objetivo**

Este libro está diseñado principalmente para:

*   **Analistas de datos** y **Científicos de datos**, especialmente aquellos en las etapas iniciales e intermedias de su carrera que necesitan fortalecer sus habilidades prácticas en preparación de datos.
*   **Ingenieros de datos** que son responsables de construir y mantener pipelines de datos robustos y que necesitan asegurar la calidad de los datos que fluyen a través de ellos.
*   **Investigadores y profesionales** en cualquier campo que trabajen regularmente con datos desordenados del mundo real y necesiten limpiarlos y prepararlos para análisis estadístico o modelado.
*   **Estudiantes** de ciencia de datos, estadística, bioinformática, etc., que buscan adquirir habilidades prácticas y fundamentales en la preparación de datos que a menudo se cubren superficialmente en otros cursos.
*   **Cualquier persona que necesite mejorar** significativamente la calidad, fiabilidad y usabilidad de sus conjuntos de datos utilizando Python.

**Conocimiento Previo Recomendado**: **Familiaridad básica con Python** (sintaxis, tipos de datos, funciones, bucles) y **conceptos introductorios de análisis de datos**. Es muy recomendable tener una **experiencia básica previa con la biblioteca Pandas** (qué es un DataFrame, selección básica), aunque el libro probablemente repasará lo esencial en el contexto de las tareas de wrangling. No es ideal como primer libro de Python o Pandas.

---

## **Estructura y Organización**

El libro sigue muy probablemente la **secuencia lógica del proceso de preparación de datos**, reflejando un flujo de trabajo realista desde los datos crudos hasta un conjunto de datos limpio y validado:

1.  **Introducción al Data Wrangling y Calidad de Datos (Cap. 1)**: Define los conceptos, explica la importancia de la calidad de los datos ("garbage in, garbage out") y presenta el alcance y las herramientas (Python, Pandas) que se utilizarán.
2.  **Adquisición de Datos (Cap. 2)**: Cubre cómo leer datos desde diversas fuentes comunes: archivos CSV, Excel, JSON, bases de datos SQL (usando bibliotecas como `sqlite3` o SQLAlchemy a nivel básico), y APIs web (usando `requests`).
3.  **Inspección y Perfilado de Datos (Cap. 3)**: Se enfoca en las técnicas iniciales para entender la estructura y la calidad de los datos recién adquiridos: uso de `.info()`, `.describe()`, visualizaciones básicas, identificación de tipos de datos, recuento de valores únicos, etc.
4.  **Manejo de Datos Faltantes (Cap. 4)**: Dedicado a identificar (`isnull()`) y tratar valores faltantes (`NaN`) utilizando diferentes estrategias: eliminación (`dropna`), imputación (media, mediana, moda, valores constantes) y posiblemente métodos más avanzados.
5.  **Limpieza de Datos Inconsistentes e Inválidos (Cap. 5)**: Aborda la corrección de errores de formato, inconsistencias textuales (mayúsculas/minúsculas, espacios), validación y corrección de tipos de datos, manejo de errores de codificación de caracteres.
6.  **Detección y Manejo de Valores Atípicos (Outliers) (Cap. 6)**: Introduce métodos para identificar valores inusuales o extremos (usando estadísticas descriptivas, reglas como IQR, o visualización) y estrategias para tratarlos (eliminación, transformación, capping).
7.  **Transformación y Remodelación de Datos (Cap. 7)**: Cubre técnicas para modificar la estructura o el contenido de los datos para el análisis: creación de nuevas características (feature engineering básico), aplicación de funciones (`apply`), normalización/escalado, discretización (`cut`), y posiblemente remodelación básica (pivotaje simple).
8.  **Validación de Datos (Cap. 8)**: Se enfoca en cómo implementar reglas y controles para asegurar que los datos limpios cumplen con ciertos criterios de calidad, integridad y coherencia (ej., rangos válidos, valores permitidos, relaciones entre columnas). Puede introducir bibliotecas de validación.
9.  **Poniéndolo Todo Junto (Cap. 9 - Posible)**: Un capítulo final que integra las técnicas aprendidas en un flujo de trabajo completo aplicado a un caso de estudio o proyecto, mostrando cómo pasar de datos crudos a limpios de manera sistemática.

La **lógica organizativa** es eminentemente **procesal**: sigue los pasos que un analista o ingeniero de datos tomaría en la práctica para preparar un conjunto de datos, abordando cada tipo de problema de calidad de datos en capítulos dedicados.

---

## **Análisis por Capítulo (Estimado y Resumido)**

*Nota: Basado en el flujo de trabajo lógico de Data Wrangling & Quality.*

---

### **Capítulo 1: El Porqué y el Qué del Data Wrangling y la Calidad**

1.  **Título y Numeración**: Capítulo 1: El Porqué y el Qué del Data Wrangling y la Calidad
2.  **Resumen Ejecutivo**: Introduce la problemática de los datos "sucios" y el impacto crítico de la calidad de los datos. Define qué es el data wrangling y sus etapas principales. Presenta Python, Pandas y NumPy como las herramientas clave que se usarán. Establece la importancia de un enfoque sistemático y reproducible. Motiva la necesidad del contenido del libro.
3.  **Objetivos Específicos**:
    *   Comprender la importancia de la calidad de los datos.
    *   Definir Data Wrangling y sus componentes.
    *   Reconocer los tipos comunes de problemas en los datos.
    *   Entender el rol de Python/Pandas en este proceso.
    *   Apreciar la necesidad de un flujo de trabajo estructurado.
4.  **Importancia Contextual**: Establece la motivación, el alcance y la relevancia del libro. Asegura que el lector comprenda por qué estas tareas son fundamentales.
5.  **Conceptos Clave**: Calidad de Datos, Data Wrangling, Datos Sucios (Messy Data), Limpieza de Datos, Transformación de Datos, Validación de Datos, Python, Pandas, NumPy, Flujo de Trabajo.
6.  **Metodología o Enfoque**: Conceptual, motivacional, introductorio.
7.  **Aplicación Práctica**: Entender el marco general del proceso de preparación de datos.
8.  **Referencia IEEE**: [1] S. E. McGregor, "Capítulo 1: El Porqué y el Qué...," en *Practical Python Data Wrangling and Data Quality*. Sebastopol, CA, USA: O'Reilly Media, 2021, pp. 1-XX (estimado).

---

### **Capítulo 2: Adquisición de Datos de Diversas Fuentes**

1.  **Título y Numeración**: Capítulo 2: Adquisición de Datos de Diversas Fuentes
2.  **Resumen Ejecutivo**: Se centra en cómo obtener datos en Python. Cubre la lectura de archivos comunes (CSV, Excel, JSON) usando Pandas (`read_csv`, `read_excel`, `read_json`). Introduce la conexión básica a bases de datos SQL para extraer datos (`read_sql`). Muestra cómo realizar solicitudes a APIs web para obtener datos usando la biblioteca `requests`.
3.  **Objetivos Específicos**:
    *   Leer archivos CSV, Excel y JSON en DataFrames de Pandas.
    *   Extraer datos de tablas de bases de datos SQL.
    *   Realizar solicitudes GET a APIs web y procesar respuestas JSON.
    *   Manejar diferentes opciones al leer datos (delimitadores, encabezados, etc.).
4.  **Importancia Contextual**: Primer paso práctico del flujo de trabajo: obtener los datos crudos. Proporciona las herramientas para trabajar con fuentes de datos realistas.
5.  **Conceptos Clave**: Adquisición de Datos, CSV, Excel, JSON, SQL, API Web, Pandas I/O (`read_*`), `requests` library.
6.  **Metodología o Enfoque**: Práctico, basado en código, mostrando cómo usar las bibliotecas relevantes para cada fuente.
7.  **Aplicación Práctica**: Ser capaz de cargar datos desde las fuentes más comunes en un entorno Python/Pandas.
8.  **Referencia IEEE**: [2] S. E. McGregor, "Capítulo 2: Adquisición de Datos...," en *Practical Python Data Wrangling...*. O'Reilly Media, 2021, pp. XX-XX.

---

### **Capítulo 3: Inspección Inicial y Perfilado de Datos**

1.  **Título y Numeración**: Capítulo 3: Inspección Inicial y Perfilado de Datos
2.  **Resumen Ejecutivo**: Una vez cargados los datos, este capítulo cubre las técnicas para obtener una comprensión inicial de su estructura y calidad. Uso de métodos de Pandas como `.head()`, `.tail()`, `.info()`, `.shape`, `.dtypes`, `.describe()`. Identificación de tipos de datos, recuento de valores faltantes (`.isnull().sum()`), valores únicos (`.nunique()`, `.value_counts()`). Visualizaciones básicas para detectar patrones o problemas (histogramas, boxplots).
3.  **Objetivos Específicos**:
    *   Obtener dimensiones y tipos de datos de un DataFrame.
    *   Calcular estadísticas descriptivas básicas.
    *   Identificar la presencia y cantidad de valores faltantes.
    *   Explorar la distribución de variables categóricas y numéricas.
    *   Utilizar métodos de Pandas para una inspección rápida y eficaz.
4.  **Importancia Contextual**: Paso fundamental después de la carga para entender con qué se está trabajando y guiar los pasos de limpieza posteriores.
5.  **Conceptos Clave**: Perfilado de Datos, Exploración de Datos (Básica), `.info()`, `.describe()`, `.dtypes`, `.isnull()`, `.nunique()`, `.value_counts()`, Estadísticas Descriptivas.
6.  **Metodología o Enfoque**: Exploratorio, utilizando funciones y métodos específicos de Pandas para resumir y entender los datos.
7.  **Aplicación Práctica**: Obtener rápidamente una visión general de cualquier nuevo conjunto de datos. Identificar áreas problemáticas que requieren limpieza.
8.  **Referencia IEEE**: [3] S. E. McGregor, "Capítulo 3: Inspección Inicial...," en *Practical Python Data Wrangling...*. O'Reilly Media, 2021, pp. XX-XX.

---

*(Resúmenes más breves para los capítulos estimados restantes basados en el flujo)*

### **Capítulo 4: Tratamiento de Datos Faltantes (Missing Data)**

*   **Resumen**: Estrategias para manejar `NaN`: identificación (`isnull`, `notnull`), visualización, eliminación (filas/columnas con `dropna`), imputación (llenar con media, mediana, moda, valor constante usando `fillna`, o métodos más sofisticados como interpolación o k-NN imputer - básico). Discusión de pros/contras de cada método.
*   **Objetivos**: Detectar/visualizar patrones de datos faltantes; Aplicar diferentes estrategias de eliminación/imputación; Entender implicaciones de cada estrategia.
*   **Contexto**: Uno de los problemas más comunes y cruciales en la limpieza de datos.
*   **Conceptos**: Datos Faltantes (`NaN`), `isnull()`, `dropna()`, Imputación, `fillna()`, Interpolación (básica).
*   **Referencia IEEE**: [4] S. E. McGregor, "Cap. 4...," *Practical Python Data Wrangling...*.

### **Capítulo 5: Limpieza de Inconsistencias y Formatos Inválidos**

*   **Resumen**: Aborda errores de entrada manual, formatos inconsistentes, problemas de codificación de texto, tipos de datos incorrectos. Técnicas: limpieza de strings (`.str` accessor, regex básico), conversión de tipos (`astype`), manejo de fechas/horas inconsistentes, estandarización de categorías.
*   **Objetivos**: Limpiar/estandarizar datos textuales; Corregir tipos de datos; Manejar formatos de fecha/hora; Asegurar consistencia en categorías.
*   **Contexto**: Trata con la "suciedad" común en datos recolectados de fuentes diversas o con entrada manual.
*   **Conceptos**: Limpieza de Strings, Expresiones Regulares (básico), Conversión de Tipos, Estandarización, `astype()`, `.str` accessor, `to_datetime()`.
*   **Referencia IEEE**: [5] S. E. McGregor, "Cap. 5...," *Practical Python Data Wrangling...*.

### **Capítulo 6: Detección y Manejo de Valores Atípicos (Outliers)**

*   **Resumen**: Métodos para identificar outliers: reglas estadísticas (ej. z-score, IQR), visualización (boxplots, scatter plots). Estrategias para manejarlos: eliminación, transformación (log, etc.), capping/winsorization, o dejarlos si son válidos.
*   **Objetivos**: Identificar outliers usando métodos estadísticos/visuales; Aplicar diferentes técnicas de tratamiento de outliers; Decidir cuándo y cómo tratar outliers.
*   **Contexto**: Los outliers pueden distorsionar análisis y modelos; su manejo requiere cuidado.
*   **Conceptos**: Valores Atípicos (Outliers), Z-score, Rango Intercuartílico (IQR), Boxplot, Capping, Winsorization, Transformación de Datos.
*   **Referencia IEEE**: [6] S. E. McGregor, "Cap. 6...," *Practical Python Data Wrangling...*.

### **Capítulo 7: Transformación y Remodelación de Datos**

*   **Resumen**: Técnicas para cambiar la forma o contenido de los datos para análisis: creación de nuevas columnas (feature engineering básico), aplicación de funciones (`apply`), binning/discretización (`cut`), normalización/escalado (usando Scikit-Learn `preprocessing` - introductorio), posible pivotaje/`melt` básico.
*   **Objetivos**: Crear nuevas características; Aplicar transformaciones complejas; Discretizar variables continuas; Normalizar/escalar datos (introducción).
*   **Contexto**: Prepara los datos limpios para análisis específicos o modelos ML.
*   **Conceptos**: Feature Engineering (básico), `apply()`, Discretización (`cut`), Normalización, Escalado, `sklearn.preprocessing` (introducción).
*   **Referencia IEEE**: [7] S. E. McGregor, "Cap. 7...," *Practical Python Data Wrangling...*.

### **Capítulo 8: Validación de Datos y Aseguramiento de la Calidad**

*   **Resumen**: Implementación de controles para verificar la calidad final: aserciones (`assert`), chequeos de rangos, validación de tipos, comprobación de valores únicos/permitidos, validación de relaciones entre columnas. Puede introducir bibliotecas como `pandera` o `great_expectations` a nivel básico.
*   **Objetivos**: Escribir código para validar la calidad de los datos; Definir reglas de validación; Usar aserciones; Introducción a bibliotecas de validación (posible).
*   **Contexto**: Paso final para asegurar que el conjunto de datos procesado es fiable y cumple con los requisitos.
*   **Conceptos**: Validación de Datos, Aserciones (`assert`), Reglas de Negocio, Integridad de Datos, `pandera` / `great_expectations` (introducción).
*   **Referencia IEEE**: [8] S. E. McGregor, "Cap. 8...," *Practical Python Data Wrangling...*.

### **Capítulo 9: Flujo de Trabajo Completo y Mejores Prácticas (Posible)**

*   **Resumen**: Integra todas las etapas (adquisición, inspección, limpieza, transformación, validación) en un flujo de trabajo cohesivo aplicado a un caso práctico. Discute mejores prácticas para reproducibilidad, documentación y mantenimiento del proceso de wrangling.
*   **Objetivos**: Aplicar el flujo de trabajo completo a un ejemplo; Entender mejores prácticas (reproducibilidad, versionado de datos - conceptual).
*   **Contexto**: Consolida el aprendizaje y enfatiza la importancia de un proceso sistemático.
*   **Conceptos**: Flujo de Trabajo de Preparación de Datos, Reproducibilidad, Documentación, Mejores Prácticas.
*   **Referencia IEEE**: [9] S. E. McGregor, "Cap. 9...," *Practical Python Data Wrangling...*.

---

## **Estrategia de Lectura Recomendada**

1.  **Secuencia Óptima**: **Altamente recomendado seguir el orden lineal de los capítulos**. La estructura sigue el flujo natural del proceso de preparación de datos, y cada capítulo se basa en los anteriores (no puedes limpiar sin inspeccionar, no puedes transformar sin limpiar, etc.).
2.  **Niveles de Lectura**:
    *   **Familiarización Rápida**: Leer introducciones y resúmenes de capítulo, ojear los ejemplos de código. Útil para entender el alcance de los problemas de calidad de datos y las técnicas generales (2-4 horas).
    *   **Lectura Profunda (Recomendada)**: Leer detenidamente, **ejecutar y experimentar con los ejemplos de código en un entorno Jupyter**. Es crucial aplicar las técnicas a datos (proporcionados o propios) para entender sus efectos y matices. Reflexionar sobre cuándo aplicar cada técnica (Estimado: 50-80 horas).
    *   **Lectura Selectiva/Referencia**: Muy útil como referencia una vez leído. Si encuentras un problema específico (ej. datos faltantes, outliers), puedes consultar directamente el capítulo correspondiente para recordar las técnicas y sintaxis.
3.  **Tiempos Estimados**:
    *   **Por Capítulo**: Estima entre 4 y 8 horas por capítulo para una comprensión sólida y práctica. Los capítulos sobre técnicas específicas de limpieza o validación pueden requerir más experimentación.
    *   **Libro Completo**: Para internalizar las técnicas y el flujo de trabajo, reserva entre **50 y 80 horas** de estudio activo y práctica.
4.  **Puntos de Conexión**:
    *   **Inspección -> Limpieza (Caps. 3 a 6)**: Constantemente relaciona los problemas identificados en la inspección con las técnicas de limpieza específicas que se aplican para resolverlos.
    *   **Limpieza -> Transformación (Caps. 4-6 a Cap. 7)**: Entiende que las transformaciones a menudo requieren que los datos ya estén relativamente limpios (ej., tipos correctos).
    *   **Todo -> Validación (Caps. 2-7 a Cap. 8)**: Reconoce que la validación debe aplicarse después de cada paso significativo de limpieza/transformación para asegurar que no se introdujeron nuevos errores.
5.  **Actividades Complementarias**:
    *   **Aplicar a Datos Reales**: La mejor forma de aprender es aplicar estas técnicas a conjuntos de datos reales y desordenados. Busca datasets en Kaggle, datos abiertos gubernamentales, o usa datos de tu propio dominio.
    *   **Construir un Pipeline Simple**: Intenta escribir un script Python que encadene varios pasos de limpieza y transformación aprendidos.
    *   **Documentar el Proceso**: Mientras limpias datos, documenta los pasos que tomaste, por qué los tomaste y los resultados. Esto refuerza el aprendizaje y la reproducibilidad.
    *   **Explorar Bibliotecas de Validación**: Si el libro las introduce, explora un poco más `pandera` o `great_expectations`.
    *   **Comparar Estrategias**: Para un problema (ej. datos faltantes), implementa y compara los resultados de diferentes estrategias (eliminar vs. imputar media vs. imputar mediana).

---

## **Lecturas Complementarias Recomendadas**

1.  **Fundamentos Previos (Python/Pandas si es necesario)**:
    *   [10] W. McKinney, *Python for Data Analysis*, 3rd ed. O'Reilly Media, 2022.
        *   *Justificación*: El libro de referencia para Pandas. Si bien este libro se enfoca en wrangling, el de McKinney cubre Pandas de forma más amplia y es un prerrequisito o co-requisito ideal.
        *   *Relación*: Proporciona la base de Pandas sobre la que se construyen las técnicas de wrangling. Cubre muchos temas de forma complementaria.
    *   [11] E. Matthes, *Python Crash Course*, 3rd ed. No Starch Press, 2023.
        *   *Justificación*: Para asegurar una base sólida en Python general antes de enfocarse en Pandas y wrangling.
        *   *Relación*: Cubre los prerrequisitos de Python.

2.  **Profundización Teórica (Calidad de Datos / Gobernanza)**:
    *   [12] T. C. Redman, *Data Driven: Profiting from Your Most Important Business Asset*. Harvard Business Review Press, 2008.
        *   *Justificación*: Un libro clásico sobre la importancia estratégica de la calidad de los datos desde una perspectiva de negocio.
        *   *Relación*: Proporciona el contexto de "por qué" la calidad de datos es crucial, más allá del "cómo" técnico del libro principal.
    *   [13] DAMA International, *DAMA-DMBOK: Data Management Body of Knowledge*, 2nd ed. Technics Publications, 2017.
        *   *Justificación*: El marco de referencia estándar para la gestión de datos, incluyendo un capítulo detallado sobre Calidad de Datos. Muy completo y formal.
        *   *Relación*: Marco teórico y de gobernanza para la calidad de datos.

3.  **Aplicaciones Prácticas (Análisis / ML Post-Wrangling)**:
    *   [14] A. Géron, *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow*, 3rd ed. O'Reilly Media, 2022.
        *   *Justificación*: Muestra qué hacer con los datos *después* de haberlos limpiado y preparado: construir modelos de ML.
        *   *Relación*: El paso siguiente natural en muchos flujos de trabajo de ciencia de datos.
    *   [15] J. VanderPlas, *Python Data Science Handbook*. O'Reilly Media, 2016 (disponible online).
        *   *Justificación*: Excelente referencia concisa que también cubre análisis y ML básico después de la manipulación de datos.
        *   *Relación*: Cubre temas posteriores al wrangling.

4.  **Perspectivas Alternativas (Herramientas de Wrangling)**:
    *   [16] Documentación de OpenRefine (https://openrefine.org/).
        *   *Justificación*: Herramienta visual potente y popular para la limpieza interactiva de datos. Ofrece una perspectiva diferente (basada en GUI) al enfoque programático de Python/Pandas.
        *   *Relación*: Enfoque alternativo/complementario para la limpieza de datos.
    *   [17] Documentación de Trifacta / Google Cloud Dataprep (Herramientas comerciales/cloud).
        *   *Justificación*: Muestra cómo se aborda el data wrangling en plataformas empresariales y de nube, a menudo con interfaces visuales y sugerencias inteligentes.
        *   *Relación*: Perspectiva industrial/empresarial sobre el data wrangling.

5.  **Desarrollos Recientes (Bibliotecas y Técnicas)**:
    *   [18] Documentación de Pandera (https://pandera.readthedocs.io/en/stable/).
        *   *Justificación*: Biblioteca popular de validación de datos para Pandas, que probablemente se mencione o complemente bien el Cap. 8.
        *   *Relación*: Profundización en validación de datos.
    *   [19] Documentación de Great Expectations (https://greatexpectations.io/docs/).
        *   *Justificación*: Otra herramienta potente y estándar de la industria para la validación, prueba y documentación de la calidad de los datos.
        *   *Relación*: Profundización y enfoque industrial en validación y calidad (Cap. 8).
    *   [20] Artículos y tutoriales sobre técnicas específicas (ej., manejo avanzado de outliers, imputación compleja) en blogs de ciencia de datos.
        *   *Justificación*: Para explorar técnicas más allá de las cubiertas en un libro introductorio/práctico.
        *   *Relación*: Profundización en temas específicos de los capítulos de limpieza/transformación.

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

[1] S. E. McGregor, "Capítulo 1: El Porqué y el Qué del Data Wrangling y la Calidad," en *Practical Python Data Wrangling and Data Quality: Getting Started with Reading, Cleaning, and Analyzing Data*. Sebastopol, CA, USA: O'Reilly Media, 2021, pp. 1-XX (estimado).

---

