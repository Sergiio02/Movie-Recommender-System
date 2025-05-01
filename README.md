# Sistema de Recomendación de Películas 🎬

## 📜 Descripción
En este proyecto, he creado **tres sistemas de recomendación diferentes** utilizando tres enfoques clásicos: 
- **Basado en popularidad** (recomendación basada en las películas más vistas o valoradas).
- **Filtrado basado en contenido** (recomendación de películas similares a aquellas que un usuario ha visto).
- **Filtrado colaborativo** (recomendación basada en el comportamiento de usuarios similares).

El objetivo es recomendar películas a los usuarios según sus gustos previos y las tendencias generales.

El proyecto inicia con un **análisis exploratorio de datos (EDA)** básico y un preprocesamiento realizado en el archivo `01_EDA.ipynb`. Luego, en el archivo `02_recommender_systems.ipynb`, se construirán los tres sistemas de recomendación.

### 🎯 Objetivos del proyecto:
- Realizar un análisis exploratorio (EDA) del dataset.
- Limpiar y preprocesar los datos.
- Desarrollar tres modelos de recomendación.

## 📊 Dataset
En este proyecto se utilizarán dos datasets:

1. The Movies Dataset: Este conjunto de datos contiene metadatos de más de 45,000 películas correspondiente a películas estrenadas hasta julio de 2017. Los datos incluyen información sobre el elenco, el equipo de producción, palabras clave del guion, presupuesto, ingresos, carteles, fechas de estreno, idiomas, compañías productoras, países, recuento de votos de TMDB y promedios de votos. Este dataset también contiene 26 millones de valoraciones de 270,000 usuarios para todas las 45,000 películas, con un rango de calificación de 1 a 5, obtenidas desde el sitio oficial de GroupLens.

2. TMDB 5000 Movie Dataset: Este conjunto contiene metadatos de aproximadamente 5,000 películas provenientes de TMDb (The Movie Database). Incluye información sobre el elenco, el equipo de producción, el presupuesto, los ingresos, las fechas de estreno, los idiomas, las compañías productoras, los países, y las valoraciones. 

Ambos datasets están disponibles en Kaggle.

## 💻 Estructura del repositorio


![Gráfico del sistema de recomendación](images/grafico_recomendador.png)
