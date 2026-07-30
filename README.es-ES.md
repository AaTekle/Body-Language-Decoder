

# Decodificador de Lenguaje Corporal

Este proyecto descifra las emociones y reacciones humanas analizando las expresiones faciales y los gestos mediante técnicas de visión por computadora y aprendizaje automático. El proyecto utiliza Python, Mediapipe, OpenCV (cv2), csv, NumPy, Pandas, scikit-learn (sklearn) y pickle para crear una herramienta que comprende el lenguaje corporal.

Idea vía @nicknochnack

![](https://github.com/AaTekle/Body-Language-Decoder/blob/main/gif/0816.gif)


## Tabla de Contenidos

- [Introducción](#introduction)
- [Descripción Técnica de Mediapipe](#technical-overview-of-mediapipe)
- [Creación del Conjunto de Datos](#creating-the-dataset)
- [Análisis de Expresiones Faciales en Tiempo Real](#real-time-facial-expression-analysis)
- [Caja/Función de Probabilidad](#probability-boxfunction)

## Descripción Técnica de Mediapipe
![MediaPipe](https://editor.analyticsvidhya.com/uploads/53474logo_horizontal_color.png)
Mediapipe, desarrollado por Google, es una biblioteca de Visión por Computadora que proporciona modelos preentrenados para diversas tareas de visión por computadora, por ejemplo, la detección de puntos faciales. Me permitió extraer fácilmente estos puntos de imágenes/flujo de vídeo, posibilitando un seguimiento preciso de puntos clave del rostro, como ojos, nariz, boca y cejas. Esta biblioteca me permite analizar e interpretar las expresiones faciales.

## Creación del Conjunto de Datos

Se necesitan datos para el preentrenamiento; utilicé el módulo `csv` para recopilar y organizar las coordenadas de los puntos faciales a través de Mediapipe. Capturé y etiqueté los puntos faciales de mis propios estados emocionales, creando un conjunto de datos. Las coordenadas se generaron en tiempo real mientras manifestaba diferentes estados emocionales; fue fascinante poder crear el conjunto de datos de manera tan interactiva en tiempo real, viendo cómo mis expresiones faciales se traducían en miles de valores numéricos (coordenadas).

## Análisis de Expresiones Faciales en Tiempo Real

OpenCV (cv2) me permitió capturar cuadros de vídeo desde la transmisión de una webcam y procesarlos utilizando el modelo de puntos faciales de Mediapipe. Las coordenadas de los puntos faciales se guardan luego en el conjunto de datos, creando una representación de las expresiones faciales (características).

## Caja/Función de Probabilidad

Utilicé NumPy para construir y mostrar una caja o función de probabilidad dentro del Decodificador de Lenguaje Corporal. Esta representación visual permite comprender la probabilidad de que se expresen diferentes emociones basándose en los datos de los puntos faciales.
