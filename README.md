# Análisis de Sentimiento (Reto Enseña x Oracle España, reto 2)
Este repositorio contiene el código necesario para entrenar y utilizar un modelo de análisis de sentimiento basado en el modelo BERT (Bidirectional Encoder Representations from Transformers).

El objetivo principal del modelo es predecir si una reseña de un producto es positiva o negativa. El modelo ha sido reentrenado con el dataset proporcionado por el Reto Enseña x Oracle España, reto 2.

## Uso
El código está diseñado para ejecutarse en Google Colab. Para utilizarlo, es necesario clonar el repositorio y abrir el notebook `analisisDeSentimiento.ipynb` en Colab.

El notebook consta de dos partes principales: entrenamiento e inferencia. En la sección de entrenamiento, se carga el dataset y se entrena el modelo. En la sección de evaluación, se cargan los datos de prueba y se evalúa el modelo en ellos.

## Resultados
Tras diferentes pruebas, hemos concluido que la red se sobreentrena de forma bastante rápida. Los mejores resultados los hemos conseguido con tan solo 3 epochs. La partición de los datos ha sido 80% para entrenamiento y 20% para validación. El resto de parámetros utilizados se pueden ver en el código.

Con todo esto, la media de resultados obtenidos ha sido de 0.9 de F1 score, siendo la mejor puntuación de 0.9099670282263035, cuyos valores se encuentran en el archivo `predictions.json`, y el modelo en la carpeta `model`.
## Notas
El repositorio también incluye el mejor modelo obtenido hasta el momento. Este modelo se puede utilizar directamente para hacer predicciones sin necesidad de entrenarlo de nuevo. Para cargar el modelo, es necesario descargarlo y cargarlo utilizando el código proporcionado en el notebook.

## Autores

Esta solcuión ha sido desarollada por los alumnos de la UAH:

- [Jesús Palomino](https://www.linkedin.com/in/jes%C3%BAs-palomino-abreu-973667218/)
- [Eduardo Ruiz Sabajanes](https://www.linkedin.com/in/eduardo-ruiz-sabajanes-23496723a/)
- [Nicolae Alexandru Molnar](https://www.linkedin.com/in/nicolae-alexandru-molnar/)
- [Oscar Garcia Azagra](https://www.linkedin.com/in/%C3%B3scar-garc%C3%ADa-azagra-ab524b258/)
- [Sergio Gala Vilda](https://www.linkedin.com/in/sergio-gala-vilda-806914262/)