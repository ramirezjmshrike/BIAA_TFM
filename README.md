# BIAA_TFM
#### Joan Manel Ramírez Jávega

Este repositorio contiene los experimentos y materiales correspondientes al Banco de Imágenes con Anotaciones de Aceras (BIAA) en el marco del Trabajo final de máster (TFM) del Máster de Ciencia de datos (UOC). Primera iteración de un proyecto para la monitorización del mantenimiento de aceras de Barcelona mediante visión computacional. Conjunto de ground truth para segmentación semántica con 507 imágenes y 10 clases.

Este paquete está conformado principalmente:

- `data/`: Carpeta que contiene CSV con metadatos de las imágenes raw data y los XLSX con los resultados experimentales de anotación manual y posprocesamiento de la preanotación con Segement Anything Model (SAM). En este [enlace](https://universe.roboflow.com/biaa/biaa_v100_gt) se pueden visualizar tanto las imágenes del conjunto ground truth y sus correspondientes máscaras.
- `source/`: Esta carpeta contiene los notebooks correspondientes a todos los experimentos realizados. Cada carpeta corresponde a un entorno de Python distinto y específico para cada experimentos y, por lo tanto, también cuenta con su correspondiente fichero `requirements.txt`:
  - `source/00_base`: Contiene los notebooks para el primer análisis exploratorio descriptivo del conjunto raw data.
  - `source/01_sam`: Contiene los notebooks del primer experimento con SAM para identificar parametrización óptima para la preanotación ajustada al caso de uso.
  - `source/02_DeepLab`: Contiene los notebooks y demás código del modelo DeepLabV3+ preentrenado con el dataset Cityscapes con el que experimentamos su capacidad para generalizar en el dominio peatonal de Barcelona y su área metropolitana.
  - `source/03_HRNer`: Contiene los notebooks y demás código del modelo HRNet preentrenado con el dataset Cityscapes con el que experimentamos su capacidad para generalizar en el dominio peatonal de Barcelona y su área metropolitana.
  - `source/04_DeepLab`: Contiene los notebooks y demás código del modelo Mask2Former preentrenado con el dataset Cityscapes con el que experimentamos su capacidad para generalizar en el dominio peatonal de Barcelona y su área metropolitana.
  - `source/05_train_DeepLab`: Contiene los notebooks y los resultados brutos (formato JSON) de los cuatro entrenamientos para el ajuste de un modelo DeepLabV3 preentrenado con Cityscapes.
- `toolkit`: Contiene los notebooks que sirvieron para realizar tareas de preprocesamiento para la rasterización de las máscaras o bien para el análisis de los resultados de la anotación manual y posprocesamiento de la preanotación con Segement Anything Model (SAM).
- `reports`: Incluye la memoria entregada del TFM.

A continuación también se detallan algunos ejemplos de segmentación obtenidas con el ajuste del modelo DeepLabV3:

<p align="center">
  <img src="figs/figs/fig_01.jpg" width="650">
</p>
<p align="center">
  <em>Figure 1: Ejemplo de segmentación número 1.</em>
</p>

<p align="center">
  <img src="figs/figs/fig_02.jpg" width="650">
</p>
<p align="center">
  <em>Figure 2: Ejemplo de segmentación número 2.</em>
</p>

<p align="center">
  <img src="figs/figs/fig_03.jpg" width="650">
</p>
<p align="center">
  <em>Figure 3: Ejemplo de segmentación número 3.</em>
</p>

<p align="center">
  <img src="figs/figs/fig_04.jpg" width="650">
</p>
<p align="center">
  <em>Figure 4: Ejemplo de segmentación número 4.</em>
</p>

<p align="center">
  <img src="figs/figs/fig_05.jpg" width="650">
</p>
<p align="center">
  <em>Figure 5: Ejemplo de segmentación número 5.</em>
</p>
