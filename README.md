# Análisis de Deserción Estudiantil

Este proyecto presenta un análisis de la deserción estudiantil a partir de la integración y procesamiento de bases de datos institucionales. El objetivo es identificar el comportamiento de las cohortes de estudiantes desde su ingreso hasta su estado actual, permitiendo evaluar la permanencia y deserción a lo largo del tiempo.

---

## Objetivo

Analizar la deserción estudiantil por cohorte y por periodo académico, mediante la construcción de una base de datos consolidada que permita:

* Realizar seguimiento longitudinal de los estudiantes
* Identificar en qué periodos se presenta mayor deserción
* Calcular tasas de deserción y supervivencia
* Determinar el número de estudiantes activos en la actualidad

---

## Fuentes de datos

El análisis se basa en la integración de dos bases de datos:

1. **Estudiantes matriculados por periodo académico**
   Contiene el historial de matrícula de los estudiantes en cada periodo.

2. **Estudiantes admitidos por periodo académico**
   Contiene información del ingreso y estado administrativo de los estudiantes.

---

## Metodología

### 1. Integración de datos

Se desarrolló un proceso en Python para:

* Limpieza y estandarización de variables
* Eliminación de registros duplicados
* Identificación del periodo de ingreso por estudiante

---

### 2. Construcción de la base de datos completa

Se generó una estructura de datos tipo:

> **Estudiante × Periodo académico**

Esto permite hacer seguimiento a cada estudiante desde su ingreso hasta su último registro, incluso en periodos donde no presenta matrícula.

---

### 3. Variables clave

La base consolidada incluye las siguientes variables principales:

* `CODIGO`: Identificador único del estudiante
* `PERIODO_INGRESO`: Periodo en el que el estudiante inicia estudios
* `PERIODO_ACADEMICO`: Periodo de análisis
* `MATRICULADO`: Indicador de matrícula en el periodo
* `ULTIMA MATRICULA`: Último periodo en el que el estudiante estuvo matriculado
* `ESTADO DEL PERIODO`: Estado académico en cada periodo
* `ESTADO_FINAL`: Estado actual del estudiante



Este proyecto permite analizar de manera integral la deserción estudiantil, proporcionando una herramienta útil para la toma de decisiones académicas y administrativas. La metodología implementada es escalable, permitiendo la actualización del análisis al incorporar nuevos periodos académicos.
