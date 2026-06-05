# Analisis_Airline_Passenger_Satisfaction

# ✈️ Análisis de Satisfacción de Pasajeros de Aerolíneas

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-green.svg)
![Plotly](https://img.shields.io/badge/Plotly-Interactive-orange.svg)

Este proyecto realiza un **Análisis Exploratorio de Datos (EDA)** profundo sobre un conjunto de datos de 103,904 pasajeros aéreos. El objetivo principal es identificar y diagnosticar los factores críticos que impactan la lealtad y la satisfacción del cliente en la industria aeronáutica.

---

## 🎯 Desafío (El Problema)
Las aerolíneas operan en un mercado altamente competitivo con márgenes financieros estrechos, donde la retención de clientes es una prioridad crítica. El problema principal radica en que la insatisfacción suele estar dispersa en múltiples métricas operativas y de servicio, dificultando la toma de decisiones. 

**El reto:** Transformar registros masivos de vuelos en *insights* accionables, aislando el "ruido" de los datos para que el equipo de operaciones sepa exactamente en qué puntos de la experiencia de viaje (logística, trámites digitales o confort a bordo) se debe invertir para maximizar la lealtad del pasajero.

---

## ⚙️ Proceso (Cómo se abordó)

El proyecto se estructuró de punta a punta dentro de un entorno de desarrollo interactivo utilizando un flujo de trabajo analítico riguroso:

1. **Exploración e Inspección Inicial (EDA):** Carga y validación del dataset utilizando **Pandas** y **NumPy** para asegurar una completitud del 100% (0 nulos relevantes y 0 duplicados).
2. **Auditoría de Lógica de Negocio:** Durante el desarrollo, se detectaron e interceptaron inconsistencias en variables preliminares (como el cruce directo de edad por distancia de vuelo), corrigiendo la lógica para evitar sesgos analíticos.
3. **Ingeniería de Variables (Feature Engineering):** Se implementaron transformaciones masivas y vectorizadas para sintetizar la información:
   * **`Service_Score`:** Un indicador consolidado que promedia las 14 calificaciones individuales de servicio en cabina y tierra.
   * **`Delay_Category`:** Segmentación inteligente de retrasos de llegada en rangos de tiempo (Corto, Medio, Largo).
   * **`Age_Group` y `Travel_Experience`:** Creación de variables categóricas para cruces demográficos y perfiles de viaje (ej. *Personal Travel - Eco*).
4. **Visualización Avanzada:** Creación de gráficos interactivos dinámicos para mapear la correlación de las características del servicio frente al indicador final de satisfacción.

---

## 📊 Resultados y Lecciones Aprendidas

* **Lección Técnica Fundamental:** La calidad de un modelo o diagnóstico depende enteramente de la fidelidad de sus reglas de negocio en el código. Validar y limpiar la lógica de las variables antes de estructurar las conclusiones salvó el proyecto de interpretaciones erróneas.
* **Impacto Operativo:** Al consolidar las 14 evaluaciones individuales en el `Service_Score` y cruzarlo con el perfil `Travel_Experience`, el análisis permite identificar con precisión quirúrgica qué segmentos específicos experimentan fricción, optimizando la asignación de presupuestos para la mejora del servicio al cliente.

---

## 🛠️ Tecnologías Utilizadas
* **Lenguaje:** Python 3.x
* **Librerías Core:** Pandas, NumPy
* **Visualización:** Plotly / Seaborn
* **Entorno:** Jupyter Notebook

---
**Desarrollado por:** Jesus Gustavo Camacho Olivos — Mayo 2026
