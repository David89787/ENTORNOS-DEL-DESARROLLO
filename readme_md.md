# Tarea: Reconocimiento de Elementos en el Desarrollo de un Programa Informático

**Autor:** David Buzón

**Módulo / Asignatura:** Programación / Fundamentos de Software

**Resultado de Aprendizaje Evaluado:**

* **RA1:** Reconoce los elementos y herramientas que intervienen en el desarrollo de un programa informático, analizando sus características y las fases en las que actúan hasta llegar a su puesta en funcionamiento.

  * *c)* Se han diferenciado los conceptos de código fuente, objeto y ejecutable.

  * *e)* Se han clasificado los lenguajes de programación.

## 🎯 Objetivo de la Tarea

Evaluar la capacidad para reconocer los elementos y herramientas que intervienen en el desarrollo de un programa informático, diferenciando los conceptos de código fuente, objeto y ejecutable, así como clasificar los lenguajes de programación en función de sus niveles de abstracción y paradigmas (imperativo y declarativo).

## 📑 Índice de Contenidos

1. [Parte 1: Análisis Teórico de Conceptos](#parte-1-análisis-teórico-de-conceptos)

   * [1. Conceptos Básicos y Ciclo de Compilación](#1-conceptos-básicos-y-ciclo-de-compilación)

   * [2. Clasificación de Lenguajes de Programación](#2-clasificación-de-lenguajes-de-programación)

2. [Parte 2: Actividad Práctica y de Análisis](#parte-2-actividad-práctica-y-de-análisis)

   * [1. Identificación de Paradigmas de Programación](#1-identificación-de-paradigmas-de-programación)

   * [2. Actividad en Grupo: Comparativa Cotidiana](#2-actividad-en-grupo-comparativa-cotidiana)

3. [Estructura del Proyecto y Entrega](#estructura-del-proyecto-y-entrega)

## Parte 1: Análisis Teórico de Conceptos

### 1. Conceptos Básicos y Ciclo de Compilación

#### Definición de Términos

* **Código Fuente:** Es el texto escrito por el programador utilizando un lenguaje de programación de alto o medio nivel (ej. C++, Java, Python). Es legible por los humanos pero no por el procesador.

* **Código Objeto:** Es el resultado de traducir (compilar) el código fuente a lenguaje máquina o instrucciones intermedias. Aún no es directamente ejecutable por el sistema operativo porque falta enlazarlo con librerías externas u otros módulos.

* **Código Ejecutable:** Es el archivo binario final que contiene todas las instrucciones en lenguaje máquina listas para ser procesadas directamente por el procesador (CPU) y gestionadas por el sistema operativo.

#### Fases de Transformación de un Programa

1. **Fase de Análisis Léxico:** El compilador lee el código fuente carácter por carácter y lo agrupa en tokens (palabras clave, identificadores, operadores).

2. **Fase de Análisis Sintáctico:** Se comprueba que los tokens sigan las reglas gramaticales del lenguaje, construyendo un árbol de sintaxis abstracta (AST).

3. **Fase de Análisis Semántico:** Se valida el significado del código (p. ej., comprobación de tipos de datos, variables no declaradas).

4. **Generación y Optimización de Código Intermedio:** Se crea un código objeto intermedio y se aplican mejoras de rendimiento.

5. **Enlazado (Linker):** Combina uno o varios archivos de código objeto con las librerías necesarias para generar el **código ejecutable**.

6. **Carga y Ejecución (Loader):** El sistema operativo carga el ejecutable en la memoria RAM y la CPU ejecuta las instrucciones.

### 2. Clasificación de Lenguajes de Programación

#### Por Nivel de Abstracción

* **Bajo Nivel:**

  * *Características:* Íntimamente ligado al hardware; ofrece control total de la memoria pero poca portabilidad.

  * *Ejemplos:* **Lenguaje Ensamblador (Assembly)** y **Código Máquina**.

* **Medio Nivel:**

  * *Características:* Ofrece estructuras de alto nivel junto con capacidades de gestión directa de memoria y punteros.

  * *Ejemplos:* **C** y **C++**.

* **Alto Nivel:**

  * *Características:* Diseñado para ser fácilmente inteligible por humanos, abstraído totalmente de las complejidades del hardware.

  * *Ejemplos:* **Python** y **Java**.

#### Por Paradigma de Programación

* **Imperativo:**

  * *Características:* Describe **cómo** debe realizarse una tarea mediante una secuencia explícita de instrucciones y cambios de estado.

  * *Ejemplos:* **C**, **Java**, **Pascal**.

* **Declarativo:**

  * *Características:* Describe **qué** resultado se desea obtener, dejando que el motor o interprete gestione los pasos internos.

  * *Ejemplos:* **SQL**, **Prolog**, **Haskell**.

## Parte 2: Actividad Práctica y de Análisis

### 1. Identificación de Paradigmas de Programación

* **Fragmento 1:** *Un programa recorre una lista de números sumándolos uno por uno.*

  * **Paradigma:** **Imperativo**

  * **Justificación:** Define detalladamente la secuencia de instrucciones y el flujo de control (controla el bucle y la acumulación estado por estado).

* **Fragmento 2:** *Una consulta SQL busca empleados mayores de 30 años y devuelve sus nombres.*

  * **Paradigma:** **Declarativo**

  * **Justificación:** Especifica el conjunto de datos que se necesita obtener sin detallar el algoritmo interno de búsqueda o indexación.

* **Fragmento 3:** *Un programa calcula el factorial definiendo el caso base (*$0! = 1$*) y la relación recursiva (*$n! = n \times (n-1)!$*).*

  * **Paradigma:** **Declarativo (Funcional / Lógico)**

  * **Justificación:** Se expresa mediante la definición matemática de relaciones y propiedades sin indicar un bucle iterativo de instrucciones explícitas.

* **Fragmento 4:** *Un programa filtra productos con precio > 10\$ recorriendo una lista elemento a elemento.*

  * **Paradigma:** **Imperativo**

  * **Justificación:** Explica explícitamente la lógica condicional y la iteración paso a paso para procesar los datos.

### 2. Actividad en Grupo: Comparativa Cotidiana

**Caso Práctico:** Preparar una taza de café espresso.

* **Enfoque Imperativo (Paso a paso):**

  1. Verter 50ml de agua en el depósito de la cafetera.

  2. Colocar 15g de café molido en el filtro.

  3. Presionar el café con el prensador a una fuerza constante.

  4. Encender la máquina y esperar a que alcance los 90°C.

  5. Activar la extracción durante 25 segundos y apagar.

* **Enfoque Declarativo (Resultado deseado):**

  * *"Quiero un café espresso corto, a 90°C, con una capa de crema consistente y servido en una taza limpia."*

#### Cuadro Comparativo

| **Criterio** | **Enfoque Imperativo** | **Enfoque Declarativo** | 
| **Ventajas** | Control preciso del proceso, fácil de depurar paso a paso. | Mayor nivel de abstracción, código más conciso y legible. | 
| **Desventajas** | Más propenso a errores manuales, código más extenso. | Menor control sobre la optimización interna del proceso. | 

## Estructura del Proyecto y Entrega

El trabajo se presenta formalmente en una presentación diapositiva/documento de entre 5 y 10 páginas que abarca:

1. Portada con datos del alumno (**David Buzón**) y del módulo.

2. Desarrollo teórico (Fases de compilación y clasificación de lenguajes).

3. Resolución analítica de los 4 fragmentos de código.

4. Trabajo en equipo y comparativa de paradigmas.