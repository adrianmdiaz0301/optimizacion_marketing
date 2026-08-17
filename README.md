# 📊 Optimización de Presupuesto y Rendimiento de Canales de Marketing

Este proyecto forma parte de mi portafolio como Analista de Datos / BI y está enfocado en diagnosticar por qué los ingresos de marketing caían pese a un mayor gasto publicitario, y en construir un modelo de reasignación de presupuesto que maximice el retorno por canal. Todo el análisis se desarrolló en Excel, simulando un caso real de una empresa retail.

## 📌 Descripción del Proyecto

**Business Question:**
¿Cómo se distribuye actualmente el presupuesto publicitario entre canales, y cómo debería reasignarse para maximizar los ingresos y el ROI, dado el desempeño histórico de cada canal?

**Metodología:**

* Limpieza y estandarización de datos crudos con Power Query (normalización de categorías, formatos de fecha, valores nulos y duplicados)
* Cálculo de métricas de desempeño por campaña: Conversion Rate, ROI, ROAS
* Consolidación de métricas por canal mediante tablas dinámicas
* Modelo de optimización de presupuesto con Solver, maximizando la ganancia proyectada sujeto a restricciones de presupuesto total
* Cruce de datos entre hojas con XLOOKUP para construir el resumen ejecutivo y el dashboard
* Visualizaciones comparativas (presupuesto/ganancia antigua vs. nueva) por canal

**Archivos principales:**
El desarrollo completo se encuentra en `Datos_Campanas_Marketing_Crudos.xlsx`, que incluye los datos crudos, los datos limpios, las tablas dinámicas, el modelo de optimización con Solver y el dashboard final.

**Impacto:**
El modelo de reasignación identifica qué canales generan mayor ganancia por sol invertido y redirige presupuesto hacia ellos, lo que en la simulación se traduce en un incremento sustancial de la ganancia total proyectada sin aumentar el presupuesto general.

## 🧠 Preguntas que respondí

📌 ¿Qué canales tienen el mejor ROI y ROAS histórico?
📌 ¿Cómo varía el desempeño de las campañas según categoría de producto, ubicación y segmento de cliente?
📌 ¿En qué etapa del embudo (Awareness, Consideration, Conversion) se concentra el gasto de cada canal?
📌 ¿Cuál es la asignación óptima de presupuesto entre canales para maximizar la ganancia total?
📌 ¿Cuánto cambiaría la ganancia proyectada si se reasigna el presupuesto según el modelo de Solver?
📌 ¿Qué relación existe entre el tipo de dispositivo, el canal y la tasa de conversión?

## 🖼️ Visualizaciones del Proyecto

A continuación, se muestran algunas de las visualizaciones generadas durante el análisis:

📌 Dashboard General

<img width="754" height="662" alt="Screenshot 2026-08-17 at 7 38 28 PM" src="https://github.com/user-attachments/assets/f2abed1a-6042-4e3b-8506-7edf324d9be8" />

📈 Modelo de Optimización con Solver

<img width="1048" height="544" alt="Screenshot 2026-08-17 at 7 39 11 PM" src="https://github.com/user-attachments/assets/fae1753e-6666-473a-b777-de01eccb0ff0" />

📊 Presupuesto y Ganancia: Antes vs. Después de la Optimización

<img width="2076" height="1338" alt="Picture1" src="https://github.com/user-attachments/assets/d8ea0f7a-50f4-4f5d-a0f6-fc81f0758865" />

## 🛠️ Herramientas y Funciones

* Excel (tablas dinámicas, gráficos dinámicos)
* Power Query (limpieza y transformación de datos)
* Solver (optimización de presupuesto sujeta a restricciones)
* XLOOKUP (cruce de datos entre hojas)

## 📁 Estructura del archivo

```
📦 optimizacion-canales-marketing
└── Datos_Campanas_Marketing_Crudos.xlsx
    ├── Datos Crudos de Campañas      # Dataset original sin procesar
    ├── Datos Limpios de Campañas     # Datos limpios + métricas calculadas (Conversion Rate, ROI, ROAS)
    ├── Pivot Table(s) - 1            # Resumen de gasto y ROI por canal
    ├── Pivot Table(s) - 2            # Resumen trimestral de presupuesto y gasto
    ├── Graficos Extras               # Comparativo de presupuesto y ganancia por canal (antes/después)
    └── Dashboard                     # Resumen ejecutivo visual
```

## 📌 Notas

* El dataset es **sintético y fue generado con IA**, diseñado para replicar patrones realistas de campañas de marketing digital (canales, segmentos, ubicaciones geográficas del Perú, dispositivos y métricas de desempeño).
* Se realizaron transformaciones como estandarización de nombres de canal y categoría, normalización de formatos de fecha y cálculo de métricas derivadas (Conversion Rate, ROI, ROAS) para facilitar el análisis.
* El modelo de Solver se configuró para maximizar la ganancia total sujeta a un presupuesto fijo y límites mínimos/máximos por canal.

## 📚 Dataset

Fuente: dataset sintético generado con inteligencia artificial, simulando campañas de marketing digital para una empresa retail peruana.

## 📬 Contacto

¡Contáctame por [LinkedIn](https://www.linkedin.com/in/adrianmdiaz/) o revisa más proyectos en mi portafolio de GitHub!
