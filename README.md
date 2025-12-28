# BIAA_TFM
#### Joan Manel Ramírez Jávega

Este repositorio contiene los experimentos y materiales correspondientes al Banco de Imágenes con Anotaciones de Aceras (BIAA) en el marco del Trabajo final de máster (TFM) del Máster de Ciencia de datos (UOC). Primera iteración de un proyecto para la monitorización del mantenimiento de aceras de Barcelona mediante visión computacional. Conjunto de ground truth para segmentación semántica con 507 imágenes y 10 clases.

Este paquete está conformado principalmente:

- `data/`: Carpeta que contiene CSV con metadatos de las imágenes raw data y los XLSX con los resultados experimentales con SAM.
- `source/`: Esta carpeta contiene los notebooks correspondientes a todos los experimentos realizados. Cada carpeta corresponde a un entorno de Python distinto y específico para cada experimentos y, por lo tanto, también cuenta con su correspondiente fichero `requirements.txt`.
- `preprocessament.ipynb`: Jupyter Notebook que inclou el codi en Python emprat per les tasques de neteja i agregació de les dades que ingereix l'app de Shiny.
- `app.R`: Aplicatiu de Shiny codificat amb R.
- També s'hi inclouen l'entregable de la presentació de la pràctica i el document amb la URL on està publicada la infografia.

En aquest [enllaç](https://ramirezjavega-jm.shinyapps.io/Analisi_comunicacions_neteja/) es pot accedir a la infografia publicada.
