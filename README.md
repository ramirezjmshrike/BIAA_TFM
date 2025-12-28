# BIAA_TFM
#### Joan Manel Ramírez Jávega

Este repositorio contiene los experimentos y materiales correspondientes al Banco de Imágenes con Anotaciones de Aceras (BIAA) en el marco del Trabajo final de máster (TFM) del Máster de Ciencia de datos (UOC). Primera iteración de un proyecto para la monitorización del mantenimiento de aceras de Barcelona mediante visión computacional. Conjunto de ground truth para segmentación semántica con 507 imágenes y 10 clases.

Este paquete está conformado principalmente:

- `data/`: Carpeta que contiene CSV con metadatos de las imágenes raw data y los XLSX con los resultados experimentales de anotación manual y posprocesamiento de la preanotación con Segement Anything Model (SAM). En este [enlace](https://universe.roboflow.com/biaa/biaa_v100_gt) se pueden visualizar tanto las imágenes del conjunto ground truth y sus correspondientes máscaras.
- `source/`: Esta carpeta contiene los notebooks correspondientes a todos los experimentos realizados. Cada carpeta corresponde a un entorno de Python distinto y específico para cada experimentos y, por lo tanto, también cuenta con su correspondiente fichero `requirements.txt`:
  - `source/00_base`: Contiene los notebooks para el primer análisis exploratorio descriptivo del conjunto raw data.
  - `source/01_sam`: Contiene los notebooks del primer experimento con SAM para identificar parametrización óptima para el presente caso de uso.
  - `source/02_DeepLab`: Contiene los notebooks y demás código del modelo DeepLabV3+ preentrenado con el dataset Cityscapes con el que experimentamos su capacidad para generalizar en el dominio peatonal de Barcelona y su área metropolitana.
  - `source/03_HRNer`: Contiene los notebooks y demás código del modelo HRNet preentrenado con el dataset Cityscapes con el que experimentamos su capacidad para generalizar en el dominio peatonal de Barcelona y su área metropolitana.
  - `source/04_DeepLab`: Contiene los notebooks y demás código del modelo Mask2Former preentrenado con el dataset Cityscapes con el que experimentamos su capacidad para generalizar en el dominio peatonal de Barcelona y su área metropolitana.
  - `source/05_train_DeepLab`: Contiene los notebooks y los resultados brutos (formato JSON) de los cuatro entrenamientos para el ajuste de un modelo DeepLabV3 preentrenado con Cityscapes.
- `preprocessament.ipynb`: Jupyter Notebook que inclou el codi en Python emprat per les tasques de neteja i agregació de les dades que ingereix l'app de Shiny.
- `app.R`: Aplicatiu de Shiny codificat amb R.
- També s'hi inclouen l'entregable de la presentació de la pràctica i el document amb la URL on està publicada la infografia.

En aquest [enllaç](https://ramirezjavega-jm.shinyapps.io/Analisi_comunicacions_neteja/) es pot accedir a la infografia publicada.
