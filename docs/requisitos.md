# 📋 Especificación de Requisitos del Sistema - Calculadora de Promedios

Este documento define las capacidades y restricciones del sistema de gestión académica, siguiendo una estructura de ingeniería de software profesional.

---

## 1. Requisitos Funcionales (RF)

### 1.1 Gestión de Datos del Estudiante
- **RF-01:** El sistema debe permitir el registro del nombre completo del estudiante.
- **RF-02:** El sistema debe permitir la creación de un catálogo de calificaciones asociadas a un estudiante, incluyendo nombre de la materia/unidad y el puntaje obtenido.
- **RF-03:** El sistema debe permitir la consulta de las notas ingresadas antes de procesar el cálculo final.

### 1.2 Procesamiento de Calificaciones
- **RF-04:** El sistema debe realizar el cálculo automático del promedio aritmético basado en la lista de notas proporcionada.
- **RF-05:** El sistema debe determinar el estatus académico (Aprobado/No Aprobado) basándose en un umbral de acreditación de 70 puntos.
- **RF-06:** El sistema debe permitir limpiar o reiniciar los datos para realizar un nuevo cálculo sin cerrar la aplicación.

### 1.3 Validación y Seguridad de Datos
- **RF-07:** El sistema debe validar que las calificaciones ingresadas sean valores numéricos.
- **RF-08:** El sistema debe restringir el rango de las notas a un intervalo de 0 a 100.
- **RF-09:** El sistema debe evitar el procesamiento de cálculos si la lista de calificaciones está vacía.

### 1.4 Visualización de Resultados
- **RF-10:** El sistema debe generar un resumen final que presente el nombre del alumno, la lista de materias, el promedio resultante y el veredicto final.

---

## 2. Requisitos No Funcionales (RNF)

### 2.1 Interfaz de Usuario
- **RNF-01:** La interfaz inicial será de tipo CLI (Interfaz de Línea de Comandos) a través de la terminal de Java.
- **RNF-02:** El sistema debe proporcionar mensajes de error claros y amigables cuando el usuario ingrese datos inválidos.
- **RNF-03 (Evolutivo):** El diseño debe estar desacoplado para permitir una futura migración a una interfaz gráfica (GUI) con Java Swing o JavaFX.

### 2.2 Entorno y Desarrollo
- **RNF-04:** El sistema debe construirse utilizando Java 17 o superior para asegurar compatibilidad con características modernas del lenguaje.
- **RNF-05:** El código debe seguir las convenciones de nomenclatura estándar de Java (CamelCase para métodos/variables y PascalCase para clases).

### 2.3 Portabilidad
- **RNF-06:** La aplicación debe ser multiplataforma, permitiendo su ejecución en sistemas Windows, macOS y Linux mediante la JVM.