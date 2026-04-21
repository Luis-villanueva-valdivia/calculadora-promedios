# 📘 Gestión de Calificaciones Académicas - Requisitos

Este documento detalla las Historias de Usuario para el sistema de cálculo de promedios, definiendo el comportamiento esperado y las reglas de negocio.

---

## Historia de Usuario No. 1
El sistema debe permitir el registro de un estudiante y la captura de sus calificaciones individuales para conformar su historial académico.

**Título:** Registro de Estudiante y Captura de Notas.

**Descripción:**
Como **estudiante**, quiero registrar mi nombre y mis calificaciones en el sistema para poder visualizar mi historial académico y preparar el cálculo de mi desempeño.

**Criterios de Aceptación:**
* **Dado que** inicio el programa, **entonces** el sistema debe solicitar y almacenar mi nombre completo.
* **Dado que** registro a un estudiante, **entonces** debe existir una opción para añadir calificaciones de forma dinámica.
* **Dado que** se visualiza el perfil del estudiante, **entonces** debe mostrarse el listado de las notas ingresadas.
* **Dado que** registro una calificación, **entonces** se debe capturar la siguiente información:
    - ID o nombre de la asignatura.
    - Valor numérico de la calificación.
* **Dado que** ingreso una nota, **entonces** el sistema debe validar que el valor esté entre **0 y 100**. Si es inválido, debe mostrar un mensaje de error y solicitar el dato nuevamente.

---

## Historia de Usuario No. 2
El sistema debe procesar las notas del estudiante para generar un resumen de rendimiento académico y estatus de acreditación.

**Título:**
Cálculo de Promedio y Estatus Académico.

**Descripción:**
Como **estudiante**, quiero procesar mis notas registradas para obtener mi promedio final y saber si he aprobado según los estándares universitarios.

**Criterios de Aceptación:**
* **Dado que** el estudiante tiene notas registradas, **entonces** debe existir una función que ejecute el cálculo del promedio aritmético.
* **Dado que** se realiza el cálculo, **entonces** el resultado debe mostrarse con un formato de **2 decimales**.
* **Dado que** el promedio es calculado, **entonces** el sistema debe asignar un estatus automático:
    - **Aprobado:** Si el promedio es mayor o igual a 70.
    - **No Aprobado:** Si el promedio es menor a 70.
* **Dado que** finaliza el proceso, **entonces** el sistema debe mostrar un resumen que incluya: Nombre, cantidad de materias evaluadas, promedio final y veredicto.