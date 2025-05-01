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

```
├── data/                       # Contiene los datasets descargados de Kaggle
│   ├── ratings_small.csv       # The Movies Dataset con valoraciones de usuarios
│   ├── tmdb_5000_movies.csv    # TMDB 5000 Movie Dataset con información básica
│   └── tmdb_5000_credits.csv   # TMDB 5000 Movie Dataset con información extendida

├── images/                     # Imágenes utilizadas para ejemplos y visualizaciones

├── notebooks/                  # Notebooks de Jupyter con análisis y modelos
│   ├── 01_EDA.ipynb            # Análisis Exploratorio de Datos (EDA)
│   └── 02_Recommender_systems.ipynb  # Desarrollo de los sistemas de recomendación

├── models/                     # Modelos entrenados guardados
│   └── modelo_svd.pkl          # Modelo de Filtrado Colaborativo (SVD)
```

## ⚙️ Requisitos

Este proyecto utiliza las siguientes librerías:

- `pandas`
- `numpy`
- `scikit-learn`
- `joblib`
- `seaborn`
- `plotly`
- `matplotlib`

## 🏁 Conclusiones

Este proyecto ha sido una excelente oportunidad para explorar diferentes enfoques de sistemas de recomendación y entender cómo cada uno puede ser útil en escenarios reales. A continuación, algunas conclusiones clave:

1. **Basado en Popularidad**: 
   Este sistema es simple y rápido de implementar, y funciona bien cuando se busca recomendar las películas más populares entre todos los usuarios. Sin embargo, no personaliza las recomendaciones y puede ser menos efectivo en ciertos contextos, como en usuarios con gustos más específicos.

2. **Filtrado Basado en Contenido**: 
   Este enfoque utiliza las características de las películas para encontrar similitudes entre ellas. Es una buena opción cuando el historial del usuario es limitado, pero puede ser limitado si las características de las películas no están bien definidas o son escasas.

3. **Filtrado Colaborativo**:
   El filtrado colaborativo es muy potente cuando se tiene una gran cantidad de datos de interacción de los usuarios, ya que es capaz de aprender patrones de comportamiento de usuarios similares. Sin embargo, puede ser costoso en términos de tiempo de cómputo y también se enfrenta a desafíos como el "cold start" (problemas cuando no hay suficiente historial de un usuario nuevo).


En general, los sistemas de recomendación pueden ser herramientas poderosas para personalizar las experiencias de los usuarios, no tiene porque haber uno que sea mejor que otro, cada uno tiene su función y además se peuden complementar, como vimos en el ejemplo de Netflix. Conviene hacer pruebas y estudiar cual funciona mejor en cada caso.


## 🤝 Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar el proyecto, por favor abre un pull request o una issue.

## 👨‍💻 Autor

- Sergio Delgado
- sergiodelamp@gmail.com
- https://github.com/Sergiio02
