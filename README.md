# X
# Análisis de Sentimiento de Tweets sobre Julián Álvarez

Este repositorio contiene el código y la documentación para realizar un análisis de sentimiento de tweets relacionados con el futbolista argentino Julián Álvarez, utilizando la API de Twitter (ahora X). El objetivo principal es comprender la opinión pública y las emociones expresadas en Twitter hacia este jugador.

## Descripción del Proyecto

Este proyecto utiliza la API de Twitter (X) para recopilar tweets que mencionan a "Julián Álvarez". Una vez recopilados los tweets, se aplica un modelo de análisis de sentimiento para clasificar cada tweet como positivo, negativo o neutral. El análisis resultante proporciona información valiosa sobre cómo se percibe al jugador en la plataforma de redes sociales.

Las etapas clave del proyecto incluyen:

* **Configuración de la API de Twitter (X):** Obtención de las credenciales necesarias para acceder a la API de Twitter.
* **Recopilación de Tweets:** Utilización de la API de Twitter para buscar y descargar tweets que contienen la frase "Julián Álvarez".
* **Preprocesamiento de Texto:** Limpieza de los tweets para eliminar ruido (menciones, hashtags, URLs, caracteres especiales, etc.) y preparar el texto para el análisis de sentimiento.
* **Análisis de Sentimiento:** Aplicación de un modelo de análisis de sentimiento pre-entrenado o el desarrollo de un modelo personalizado para clasificar el sentimiento de cada tweet.
* **Visualización y Análisis de Resultados:** Presentación de los resultados del análisis de sentimiento mediante gráficos y estadísticas para obtener información sobre la distribución de sentimientos.

## Conjunto de Datos

El conjunto de datos utilizado en este proyecto se genera dinámicamente mediante la consulta a la API de Twitter (X) en tiempo real (o en un período de tiempo específico). Cada tweet recopilado contendrá información como:

* Texto del tweet
* Fecha y hora de creación
* Autor del tweet (nombre de usuario, ID)
* Número de retweets
* Número de likes
* Otros metadatos proporcionados por la API de Twitter.

**Nota:** El acceso a la API de Twitter (X) puede requerir una cuenta de desarrollador y la obtención de claves de API. Las políticas de la API pueden cambiar, por lo que es importante consultar la documentación oficial de Twitter para desarrolladores.

## Estructura del Repositorio

├── README.md
├── notebooks/
│   └── analisis_sentimiento_alvarez.ipynb  # Notebook de Jupyter con el código del análisis
├── src/
│   ├── twitter_api.py                  # Código para interactuar con la API de Twitter
│   ├── sentiment_analysis.py           # Código para realizar el análisis de sentimiento
│   ├── preprocessing.py              # Código para preprocesar los tweets
├── data/
│   ├── raw_tweets.json               # Tweets sin procesar (opcional)
│   └── sentiment_results.csv         # Resultados del análisis de sentimiento (opcional)
├── models/
│   └── sentiment_model.pkl           # Modelo de análisis de sentimiento (si se entrena uno)
└── requirements.txt                  # Lista de dependencias de Python

## Tecnologías Utilizadas

* **Python:** Lenguaje de programación principal utilizado para la interacción con la API y el análisis de datos.
* **Tweepy:** Biblioteca de Python para interactuar con la API de Twitter (X).
* **NLTK (Natural Language Toolkit) o spaCy:** Bibliotecas de Python para el procesamiento del lenguaje natural (tokenización, lematización, etc.).
* **Transformers (Hugging Face):** Biblioteca de Python que proporciona modelos pre-entrenados para diversas tareas de PLN, incluyendo el análisis de sentimiento.
* **TextBlob o VADER (Valence Aware Dictionary and sEntiment Reasoner):** Librerías de Python para el análisis de sentimiento léxico.
* **Pandas:** Biblioteca de Python para la manipulación y el análisis de datos tabulares.
* **Matplotlib y Seaborn:** Bibliotecas de Python para la visualización de datos.
* **Jupyter Notebook/Lab:** Entorno interactivo para escribir y ejecutar código.
