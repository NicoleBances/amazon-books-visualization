# Análisis y Visualización de los Libros Más Vendidos en Amazon (2009-2019)

---

## Colaboradores

- Francesca Nicole Bances Torres 
- Marsi Valeria Figueroa Larragán
  
---

## Resumen

Este proyecto analiza los datos de los **50 libros más vendidos en Amazon** entre 2009 y 2019, utilizando el dataset *“Amazon Top 50 Bestselling Books”*. Se aplicaron procesos de **limpieza, transformación y visualización de datos** en un entorno colaborativo (Google Colab).  

Se plantearon tres hipótesis sobre la relación entre precio, calificación, género y permanencia en el ranking. Las visualizaciones permitieron identificar patrones y validar o rechazar estas hipótesis, proporcionando una comprensión profunda del comportamiento de los bestsellers en Amazon.  

El proyecto permitió aplicar herramientas de análisis exploratorio y desarrollar habilidades en **pensamiento crítico** e interpretación de datos basadas en evidencia visual.

---

## Objetivo del Estudiante (Student Outcome)

- Desarrollar la capacidad para comprender y brindar soporte en la entrega de sistemas de información en entornos tecnológicos.  
- Aplicar técnicas de limpieza y visualización para explorar información y validar hipótesis.  
- Fortalecer competencias en preparación, manipulación y análisis de datos para la toma de decisiones basada en evidencia.  

---

## Misión del trabajo

- Crear un **dashboard interactivo y funcional** que comunique patrones, tendencias y relaciones significativas de los libros más vendidos.  
- Aplicar el **ciclo completo de visualización de datos**: comprensión del problema, exploración del dataset, limpieza, transformación, selección de gráficos y validación de resultados.  
- Generar conocimiento útil sobre calificaciones, precios, permanencia en rankings, géneros y autores, promoviendo el **storytelling visual** y la síntesis de información.  

---

## Objetivo de la presentación

- Presentar visualizaciones claras e intuitivas que permitan a Amazon identificar patrones clave y oportunidades de negocio.  
- Evaluar y sustentar mediante evidencia visual las siguientes hipótesis:  

  1. **H1:** Los libros más baratos tienden a recibir mejores calificaciones.  
  2. **H2:** Existen géneros que consistentemente obtienen buenas calificaciones, destacando la ficción.  
  3. **H3:** Una buena calificación sostenida contribuye a que un libro permanezca más años en el ranking de los más vendidos.  

---

## Contexto

- Amazon busca fortalecer sus estrategias comerciales en libros digitales, entendiendo mejor los hábitos de lectura.  
- El dataset contiene **550 registros** y **7 variables clave**: nombre del libro, autor, calificación, reseñas, precio, año y género.  

### Dataset

- **Nombre:** Amazon Top 50 Bestselling Books 2009–2019  
- **Fuente:** [Kaggle](https://www.kaggle.com/datasets/sootersaalu/amazon-top-50-bestselling-books-2009-2019)  
- **Registros:** 550  
- **Variables:** 7  

| Variable      | Tipo       | Descripción                                      | Posibles valores                     |
|---------------|-----------|-------------------------------------------------|-------------------------------------|
| Name          | Categórico | Nombre del libro                                | Texto                               |
| Author        | Categórico | Autor                                           | Texto                               |
| User Rating   | Numérico   | Calificación promedio de usuarios              | 0.0 – 5.0                           |
| Reviews       | Numérico   | Número de reseñas                              | Enteros positivos                   |
| Price         | Numérico   | Precio del libro                               | 0 – 105                             |
| Year          | Numérico   | Año del ranking                                | 2009 – 2019                         |
| Genre         | Categórico | Género del libro                               | Fiction / Non Fiction               |

---

## Dashboard

- Desarrollado con **Streamlit**, permite visualizar datos de forma interactiva y accesible.  
- Funcionalidades:
  - Filtrar por año, género o autor.  
  - Comparar precios, calificaciones y permanencia en rankings.  
  - Visualizar patrones y tendencias clave para decisiones estratégicas.  

**Link al dashboard:** [https://tf-data-visualization.streamlit.app/](https://tf-data-visualization.streamlit.app/)  

---

## Hipótesis y resultados

### H1: Los libros más baratos son mejor calificados

- Alta concentración de libros entre 0–20 unidades con calificaciones de 4.2–4.8.  
- La línea de tendencia descendente indica que **a mayor precio, menor calificación promedio**.  
- **Conclusión:** H1 aceptada. Los libros baratos tienden a recibir mejores calificaciones.  

### H2: Existen géneros que siempre serán bien calificados

- Ficción: mediana de calificación 4.7, con mayor dispersión y algunos outliers bajos.  
- No Ficción: mediana 4.6, más consistente y menos dispersión.  
- **Conclusión:** H2 aceptada. La ficción suele recibir mejores calificaciones promedio, aunque ambos géneros son bien valorados.  

### H3: Una buena calificación sostenida mantiene a un libro en el ranking

- Libros con calificaciones altas (≥4.5) tienden a aparecer en el ranking varios años.  
- Correlación positiva débil entre calificación promedio y permanencia.  
- **Conclusión:** H3 aceptada. La calificación alta ayuda a mantener libros en el ranking de ventas, aunque no garantiza permanencia absoluta.  

---

## Visualizaciones utilizadas

| Tipo de gráfico       | Propósito                                                                 |
|----------------------|--------------------------------------------------------------------------|
| Heatmap               | Detectar valores nulos.                                                  |
| Countplot / Barplot   | Frecuencia de calificaciones, géneros y autores.                        |
| Boxplot               | Distribución de precios, reseñas y calificaciones por género.            |
| Lineplot              | Evolución de reseñas y calificaciones a lo largo del tiempo.             |
| Scatterplot / Regplot | Relación entre precio y calificación promedio.                           |

- Librería principal: **Seaborn** (Waskom, 2021)  

---

## Recomendaciones

- Crear un **dashboard dinámico** con filtros interactivos por año, género y autor.  
- Incorporar pruebas estadísticas formales para fortalecer la validez de los hallazgos.  
- Automatizar y documentar mejor los pasos de preprocesamiento para replicabilidad y profesionalismo.  


