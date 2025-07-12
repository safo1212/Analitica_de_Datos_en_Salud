# Analítica de Datos en Salud

Este repositorio contiene los desarrollos realizados en Colab para actividades y tareas de analítica de datos aplicada al sector salud.

Presentado por:

* 2400452 - Jennifer Benavides Castillo  
* 2400479 - Cristhian David Cruz Millán  
* 2400794 - Sergio Alejandro Fierro Ospitia  
* 2400478 - Edwin Andrés Lasso Rosero  

---

## Tarea 1: Extracción de Conceptos Médicos (Fine-Tuning con cáncer de pulmón)

Desarrollar una herramienta basada en fine-tuning de un modelo de lenguaje natural para identificar automáticamente entidades médicas relevantes en historias clínicas de pacientes con cáncer de pulmón.

**Actividades realizadas:**

- Procesamiento de un corpus clínico anotado en formato BIO para entrenamiento de un modelo NER.
- Afinamiento de un modelo preentrenado (transfer learning) especializado en lenguaje clínico.
- Script de entrenamiento documentado (`Entregable 1`) para adaptar el modelo al dominio médico.
- Script de validación (`Entregable 2`) para evaluar el modelo con nuevas oraciones clínicas.
- Evaluación del desempeño del modelo en tareas de extracción de entidades médicas.

---

## Tarea 2: Aplicación de Extracción de Información (Integración de modelos en cáncer de mama)

Construcción de una aplicación que procese historias clínicas de pacientes con cáncer de mama, extrayendo entidades médicas y clasificando su contexto (afirmativo, negado o incierto).

**Actividades realizadas:**

- Aplicación de un modelo NER entrenado en lenguaje biomédico sobre textos clínicos (`Entregable 1`).
- Implementación de un modelo de clasificación de contexto para detectar negación, afirmación e incertidumbre (`Entregable 2`).
- Integración de ambos modelos en un flujo de procesamiento conjunto (`Entregable 3`).
- Generación de una base de datos estructurada (formato CSV) con:
  - `patient_id`: Identificador del paciente.
  - `sentence`: Oración original.
  - `NER`: Entidad médica extraída.
  - `Estado`: Contexto de la entidad (Afirmada, Negada, Sospechosa).