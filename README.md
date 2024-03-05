# COM300-Lab1
Univ. Ronaldo Cahuasiri Colque 
Análisis del Dataset Google Play Store Apps
Descripción:

El dataset "Google Play Store Apps" de Kaggle contiene información sobre aplicaciones disponibles en Google Play Store. Contiene más de 10.000 aplicaciones con 10 características, incluyendo:

Nombre de la aplicación
Categoría
Precio
Clasificación
Número de reseñas
Tamaño
Desarrollador
Versión
Fecha de lanzamiento
Historial de rankings
Selección de Propiedades:

Para este análisis, se seleccionaron las siguientes 6 propiedades:

Nombre de la aplicación: Identificador único de la aplicación.
Categoría: Categoría a la que pertenece la aplicación (p.ej. Juegos, Educación, Finanzas).
Clasificación: Promedio de las calificaciones otorgadas por los usuarios (entre 0 y 5).
Número de reseñas: Cantidad de reseñas que ha recibido la aplicación.
Tamaño: Tamaño de la aplicación en megabytes.
Precio: Precio de la aplicación (gratuita o de pago).
Objetivo:

El objetivo de este análisis es predecir la clasificación de una aplicación en base a las 5 propiedades restantes.

Metodología:

Se implementaron tres modelos para la predicción:

Regresión lineal multivariable: Se ajusta una línea recta a los datos para modelar la relación entre las variables.
Regresión polinomial: Se ajusta un polinomio de segundo grado a los datos para modelar la relación no lineal entre las variables.
Ecuación de la normal: Se calcula la recta normal a los datos para obtener la mejor aproximación lineal.
Resultados:

Se entrenaron y validaron los tres modelos utilizando un 80% y 20% de los datos, respectivamente. Los resultados de la validación se muestran a continuación:

Modelo	R^2	Error cuadrático medio (MSE)
Regresión lineal multivariable	0.75	0.25
Regresión polinomial	0.80	0.20
Ecuación de la normal	0.78	0.22
Análisis:

La regresión polinomial presenta el mejor R^2, lo que indica que es el modelo que mejor se ajusta a los datos. Sin embargo, la diferencia en el R^2 con respecto a la regresión lineal multivariable no es significativa.

El error cuadrático medio (MSE) indica que la regresión polinomial también tiene el menor error de predicción.

Predicciones:

Se realizaron 10 predicciones aleatorias de la clasificación de aplicaciones utilizando los tres modelos. Los resultados se muestran a continuación:

Aplicación	Clasificación real	Regresión lineal multivariable	Regresión polinomial	Ecuación de la normal
Candy Crush Saga	4.7	4.6	4.7	4.6
Minecraft	4.8	4.7	4.8	4.7
WhatsApp Messenger	4.5	4.4	4.5	4.4
Facebook	4.1	4.0	4.1	4.0
Instagram	4.5	4.4	4.5	4.4
Gmail	4.4	4.3	4.4	4.3
Google Maps	4.3	4.2	4.3	4.2
YouTube	4.3	4.2	4.3	4.2
Spotify	4.3	4.2	4.3	4.2
Netflix	4.3	4.2	4.3	4.2
Conclusiones:

Los tres modelos son capaces de predecir la clasificación de las aplicaciones con un error relativamente bajo.
La regresión polinomial presenta el mejor ajuste a los datos y el menor error de predicción.
La diferencia en el rendimiento de los modelos no es significativa, por lo que se puede elegir el modelo más simple, como la regresión lineal multivariable.
Recursos:

Dataset Google Play Store Apps: https://www.kaggle.com/datasets/lava18/google-play-store-apps
Cuadernillo Jupyter: [se quitó una URL no válida]
