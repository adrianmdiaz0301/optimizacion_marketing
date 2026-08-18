# 📊 Optimización de Presupuesto y Rendimiento de Canales de Marketing

Este proyecto forma parte de mi portafolio como Analista de Datos / BI y está enfocado en diagnosticar por qué los ingresos de marketing caían pese a un mayor gasto publicitario, y en construir un modelo de reasignación de presupuesto que maximice el retorno por canal. Todo el análisis se desarrolló en Excel, simulando un caso real de una empresa retail.

## 📌 Descripción del Proyecto

**Business Question:**
El gasto en marketing creció de forma sostenida este año, pero el ROI general no acompañó ese crecimiento. ¿Qué canal(es) están arrastrando el desempeño general, y hacia dónde debería reasignarse el presupuesto?

**Metodología:**

* Limpieza y estandarización de datos crudos con Power Query (normalización de categorías, formatos de fecha, valores nulos y duplicados)
* Cálculo de métricas de desempeño por campaña: Conversion Rate, ROI, ROAS
* Consolidación de métricas por canal mediante tablas dinámicas
* Análisis de desempeño y atribución por etapa del embudo: en lugar de simplemente eliminar los canales de bajo rendimiento (plan original), identifiqué que el "bajo rendimiento" era en realidad un problema de atribución — se estaba evaluando a los canales de awareness (parte alta del embudo) con ROI, cuando la métrica correcta para esa etapa es ROAS
* Modelo de optimización de presupuesto con Solver, redistribuyendo el gasto para maximizar tanto la ganancia como las impresiones, de modo que se generen más ingresos sin sacrificar las métricas de la parte alta del embudo
* Cruce de datos entre hojas con XLOOKUP para construir el resumen ejecutivo y el dashboard
* Visualizaciones comparativas (presupuesto/ganancia antigua vs. nueva) por canal

**Archivos principales:**
El desarrollo completo se encuentra en `Simulacion_Datos`, que incluye los datos crudos, los datos limpios, las tablas dinámicas, el modelo de optimización con Solver y el dashboard final. El slide deck se encuentra en `Simulacion_Slide_Deck` que contiene el pitch final. 

**Impacto:**
Al corregir la métrica de atribución por etapa del embudo y redistribuir el presupuesto en función del retorno real de cada canal, el modelo proyectó un incremento de **S/6.3 millones** en la ganancia total, manteniendo (e incluso protegiendo) las impresiones de los canales de awareness, sin aumentar el presupuesto general.

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

<img width="754" height="662" alt="Screenshot 2026-08-17 at 7 38 28 PM" src="https://github.com/user-attachments/assets/786e5882-fe61-4cf2-bc4e-9a5cc6b7d165" />

📈 Modelo de Optimización con Solver

<img width="1048" height="544" alt="Screenshot 2026-08-17 at 7 39 11 PM" src="https://github.com/user-attachments/assets/6669e145-6fab-460b-9b22-37397bdf0458" />

📊 Presupuesto y Ganancia: Antes vs. Después de la Optimización

<img width="2076" height="1338" alt="Picture1" src="https://github.com/user-attachments/assets/4db9ad69-1331-4a4c-a0c2-bbea1ddd2d52" />

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

¿Tienes sugerencias o quieres colaborar?
¡Contáctame por [LinkedIn](https://www.linkedin.com/in/adrianmdiaz/) o revisa más proyectos en mi portafolio!
