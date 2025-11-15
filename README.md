# Detección de criaderos de mosquitos a partir de imágenes aéreas con drones

Este proyecto corresponde a mi **tesis de maestría** y tiene como objetivo desarrollar un sistema capaz de detectar automáticamente posibles criaderos de mosquitos (como cubetas, llantas desechadas, tinacos, macetas y charcos) a partir de imágenes aéreas capturadas con drones.

El trabajo se enmarca en una iniciativa del **Instituto Nacional de Salud Pública (INSP)**, cuyo propósito es contribuir a la reducción de enfermedades transmitidas por mosquitos —como chikungunya, zika y dengue— en México. En colaboración con el **CIMAT**, se han desarrollado diversos subproyectos de investigación, entre ellos el presente.

El INSP recolectó imágenes aéreas de **alta resolución** mediante drones en la ciudad de **Tapachula, Chiapas**, una zona fuertemente afectada por dichas enfermedades. Estas imágenes incluyen techos de viviendas, patios, calles y otros espacios urbanos. A partir de esta información se generó una base de más de **5,000 imágenes etiquetadas manualmente**, que sirvió para entrenar y evaluar diferentes modelos de detección de objetos de última generación.

A futuro, se busca que este sistema pueda integrarse en drones que sobrevuelen zonas de interés y detecten criaderos en tiempo real. Esto permitiría recolectar datos de manera eficiente y, al mismo tiempo, facilitar la eliminación oportuna de criaderos, contribuyendo así a **controlar o prevenir la proliferación de mosquitos**.

---

## Problemática
Las enfermedades transmitidas por mosquitos representan uno de los principales problemas de salud pública en México y en el mundo. El mosquito es considerado el animal que más muertes ocasiona a nivel global cada año.

## Objetivo
Desarrollar un sistema de visión por computadora que detecte de forma automática diferentes tipos de criaderos de mosquitos a partir de imágenes aéreas capturadas por drones.

## Enfoque de solución
Se implementaron **redes neuronales convolucionales** de la familia **YOLO (You Only Look Once)**, dado su buen equilibrio entre precisión y velocidad, una característica fundamental para este proyecto en escenarios de inferencia en tiempo real.

Los modelos evaluados incluyen:
- YOLOv4-tiny
- YOLOv4
- YOLOv7-tiny
- YOLOv7x
- YOLOv8n
- YOLOv8x
- YOLOv12n
- YOLOv12x

## Resultados
Los experimentos muestran resultados satisfactorios. El mejor desempeño se obtuvo con **YOLOv12x**, alcanzando un **mAP@50 de 78%** en precisión.

## Archivos del repositorio
- **marco_teorico_modelos.pdf**  
  Contiene la descripción teórica y la arquitectura de los modelos seleccionados.

- **implementaciones_modelos_YOLO.pdf**  
  En este proyecto aún no se comparte código pero se explica los requerimientos computacionales y el proceso detallado de implementación de los modelos YOLO utilizados en español.

- **metodologia_tesis.pdf**  
  Presenta la metodología seguida en el desarrollo de la tesis.

- **experimentos_resultados.pdf**  
  Resume los resultados obtenidos en los experimentos realizados.

---

## Notas importantes
- Además de la base de datos proporcionada por el INSP, se utilizó otra base pública de características similares disponible en línea.  
- Aunque los resultados de la tesis ya se encuentran completos, en este repositorio solo se muestra una parte de ellos por motivos de **confidencialidad**, dado que se busca publicar un artículo académico.  
- Una vez publicado el artículo, se liberarán públicamente la **base de datos etiquetada**, el **código implementado** y el resto de los resultados.
- 

[Predicciones 1](image_x5_207.jpg)
[Predicciones 1](image_x5_7429.jpg)
[Predicciones 1](image_x5_7476.jpg)
