# Curso CoderHouse Data Science

👋 Bienvenido/da

# Desafios

- Los desafios completados del Curso son los siguientes:

## Desafio Evaluando modelos de Machine Learning

- Requerimientos:

    - Realizar una segunda ronda de Feature Engineering con el fin de ampliar el número de variables incluidas en el modelo MVP de la entrega anterior.

        -   Al nuevo data set se agregan las variables:

            - Sh (Shots): Número total de tiros realizados por un jugador.

            - SoT (Shots on target): Número total de tiros que han ido a puerta.

            - SoT% (Shots on target percentage): Porcentaje de tiros que han ido a puerta.

            - Sh/90 (Shots per 90 minutes): Número medio de tiros realizados por un jugador por partido.

            - SoT/90 (Shots on target per 90 minutes): Número medio de tiros que han ido a puerta por partido.

            - G/Sh (Goals per shot): Número medio de goles marcados por un jugador por cada tiro realizado.

            - G/SoT (Goals per shot on target): Número medio de goles marcados por un jugador por cada tiro que ha ido a puerta.

            - Dist (Distance): Distancia media de los tiros realizados por un jugador.

            - FK (Free kicks): Número total de tiros libres realizados por un jugador.

            - npxG/Sh (Non-penalty expected goals per shot): Número medio de goles esperados por un jugador por cada tiro realizado, excluyendo los goles marcados desde el punto de penalti.

    - Realizar una segunda ronda de entrenamiento con más variables.

    Los resultados obtenidos para el nuevo dataset (modelo 2) son:

        - feature selection - Selección de caracteristicas univariadas - Regresión Lineal - Variable Gls (Goles):
        
            - Mean Squared Error (MSE): 3.3632029571995354e-06
            - R-squared (R2): 0.999999720098907

        - feature selection - Selección de caracteristicas univariadas - Regresión Lineal - Variable Ast (Asistencias):

            - Mean Squared Error (MSE): 5.851615851581933e-29
            - R-squared (R2): 1.0

    - Comparar la performance de ambos modelos en el conjunto de testeo.

        - Modelo 1: Resultados de Desafio Anterior
        - Modelo 2: Resultados de Actual Desafio, con incorporacion de nuevas variables

        - Resultados de comparación:

            - Variable Goles: 
                    - El modelo 2 es mejor que el modelo 1 en términos de MSE.
                    - La mejora es de un 20%.
                    - El modelo 2 es más complejo y requiere más datos para entrenar.
            
            - Variable Asistencias:
                    - En un conjunto de testeo, los modelos de regresión lineal para predecir asistencias de jugadores tienen un MSE muy bajo y un R2 muy alto. 
                    - El modelo 1 es ligeramente más preciso que el modelo 2.

- Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/Desafio_EvaluacionML_Luis+Solis.ipynb

## Desafio Entrenando un algoritmo de Machine Learning

- Requerimientos:

    - Utilizar una fuente de datos para resolver problemas de clasificación o regresión.

    - Realizar los procesos de Encoding, Feature Engineering y entrenamiento de un modelo de Machine Learning (Clasificación o Regresión).

    - Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/Desafio_AlgoritmoML_MVP_Luis_Solis.ipynb


## Desafio Segunda Pre entrega:

- Requerimientos:

    - Generar insights que permitan dar respuesta a las preguntas por responder.

    - Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/SegundaPreEntregaProyectoFinal+Solis.ipynb

## Desafio Obtención de insights:

- Requerimientos:

    - Generar insights que permitan dar respuesta a las preguntas por responder.

    - Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/Obtencion_de_insights+Solis.ipynb


https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/Análisis_Datos_Fútbol.pptx

## Desafio Data Storytelling:

- Requerimientos:

    - Iniciar el proceso de Data Storytelling respondiendo las preguntas que se quieran responder.

    - Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/Data_Storytelling+Solis.ipynb

## Desafio Data Wrangling:

- Requerimientos:

    - Iniciar el proceso de limpieza y exploración de datos según el dataset elegido para el proyecto final.

    - Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/Data_Wrangling+Solis.ipynb

- Consideraciones:

    - Se encontro un valor NaN - fila 1875, columna "Nation", para player David Ozoh. Se cambia por valor "ENG", correspondiente a nacional England.

    - Se encuentra 105 valores con nombres de jugadores que contienen caracter "?". Ejemplo: 
        - Fila: 95, columna: Player, valor: Komnen Andri? 
        - Nombre Correcto:  'Komnen Andrić'

        - Se cambian los valores de los 105 nombres.

## Descarga de datos desde APIs publicas

- Requerimientos:

    - Buscar información en APIs públicas (i.e Twitter, NewsAPI, Spotify, Google Apis, etc).
    - Extraer datos e importarlos a un dataframe realizando una exploración simple (i.e filas, columnas, tipos de datos).

- Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/Desafio_APIS_Luis+Solis.ipynb

## Primera Entrega Proyecto Final

- Requerimientos:

    - Estructurar un problema en función de múltiples, pero simples preguntas/hipótesis a responder
    - Analizar datos tabulares (e.g excel, csv, etc)  usando Python
    - Utilizar modelos de Machine Learning con Python

- Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/ProyectoFinal+LSolis.ipynb

- Consideraciones:

    - Lo analizado en Archivo ProyectoFinal+LSolis.ipynb es un compilado de los desafios anteriores.
    - Se selecciona modelo Random Forest ya que tiene mejor performance que modelo Elastic Net, de acuerdo a lo analizado en el desafio anterior.

## Desafio Complementario Evaluando Modelos ML

- Requerimientos:

    - Generar una evaluación de modelos apropiados para el problema de interés.
    - Identificar por medio de las métricas generadas si se puede tener una situación de overfitting (sobreajuste) o underfitting (subajuste), discutiendo posibles formas de mejora

- Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/ProyectoDS_ParteIII_Solis_III.ipynb

- Consideraciones:

    - Se implementaron modelos Random Forest y Elastic Net. Resultados:

        - Random Forest: 
            - Error cuadrático medio (MSE) - Conjunto de entrenamiento: 3.420932607883566
            - Error cuadrático medio (MSE) - Conjunto de prueba: 2.903501202996976
            - Coeficiente de determinación (R^2) - Conjunto de entrenamiento: 0.16256611515822927
            - Coeficiente de determinación (R^2) - Conjunto de prueba: 0.2603353991224575
            - Error absoluto medio (MAE) - Conjunto de entrenamiento: 0.31082945339684603
            - Error absoluto medio (MAE) - Conjunto de prueba: 0.399162829832605

        - Elastic Net:
            - Error cuadrático medio (MSE) - Conjunto de entrenamiento: 3.420932607883566
            - Error cuadrático medio (MSE) - Conjunto de prueba: 2.903501202996976
            - Coeficiente de determinación (R^2) - Conjunto de entrenamiento: 0.16256611515822927
            - Coeficiente de determinación (R^2) - Conjunto de prueba: 0.2603353991224575
            - Error absoluto medio (MAE) - Conjunto de entrenamiento: 0.31082945339684603
            - Error absoluto medio (MAE) - Conjunto de prueba: 0.399162829832605

    - Conclusiones:
        Comparando los Modelos Finales de Random Forest y Elastic Net, el modelo Random Forest parece ser una mejor elección en comparación con el modelo Elastic Net. Esto se debe a que el modelo Random Forest presenta valores más bajos de error cuadrático medio (MSE) tanto en el conjunto de entrenamiento como en el conjunto de prueba, lo que indica una mejor capacidad de predicción y ajuste a los datos. Además, el coeficiente de determinación (R^2) es más alto en el modelo Random Forest, lo que indica que este modelo explica una mayor proporción de la varianza en los datos objetivo.

## Desafio Estructurando un Proyecto de DS (parte III)

- Requerimientos:

    - Crearán un notebook que complemente el trabajo realizado en los siguientes apartados: 
        - elegir un método de feature selection para reducir la dimensionalidad del dataset, 
        - elegir un algoritmo de regresión o clasificación para entrenar con los datos elegidos,
        - cálculo de métricas para validar el modelo
        - generar conclusiones con base en los resultados obtenidos.

- Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/ProyectoDS_ParteIII_Solis.ipynb

- Consideraciones:

    - Se implemento dos selección de caracteristicas ( Correlación Pearson y Univariadas - Correlación Lineal)
    - Se requiere una evaluación adicional y considerar otros modelos para mejorar el rendimiento de los modelos planteados.

- Archivo Adicional Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/ProyectoDS_ParteIII_Solis_bis.ipynb

    - Se implementaron dos modelos adicionales (Random Forest y Elastic Net). Los resultados obtenidos son los siguientes:

        - Random Forest:
            - Coeficiente de determinación (R^2): 0.6992567213869347
            - Precisión en la predicción de los valores objetivos: 0.7936802973977695
            - Error absoluto medio (MAE): 0.40715663539269487 

            Conclusiones: Los resultados indican que el modelo de Random Forest tiene una capacidad moderada para explicar y predecir los valores objetivo, con un R^2 de 0.699 y una precisión del 79.4%. El MAE de 0.407 muestra una diferencia promedio entre los valores reales y las predicciones.

        - Elastic Net:
            - Coeficiente de determinación (R^2): 0.14922875008453873
            - Precisión en la predicción de los valores objetivos: 0.14922875008453873
            - Error absoluto medio (MAE): 1.042423816912241

            Conclusiones: El modelo de Elastic Net con las variables seleccionadas explica solo el 14.92% de la variabilidad de la variable objetivo. La precisión en la predicción es baja y las predicciones tienen un error medio de 1.0424 unidades en la escala de la variable objetivo.


## Desafio Estructurando un Proyecto de DS (parte II)

- Requerimientos:

    - Abstracto con motivación y audiencia
    - Preguntas/Hipótesis que queremos resolver mediante el análisis de datos
    - Análisis Exploratorio de Datos (EDA)
    - Con base en las visualizaciones y resúmenes numéricos generados del desafío anterior dar recomendaciones basados en los insights observados.
    - Para esta oportunidad deberás tener avances en los apartados: Definición de objetivo, Contexto comercial, Problema Comercial, Contexto analítico, Exploración de datos (EDA)

Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/ProyectoDS_ParteII_Solis.ipynb

## Desafio Estructurando un Proyecto de DS (parte I)

- Requerimientos:

    - Generar preguntas de interés o hipótesis de interés sobre el dataset elegido para el proyecto final.
    - Crear visualizaciones (univariados, bivariados o trivariados) junto con resúmenes numéricos básicos acordes con los tipos de variables disponibles.
    - Interpretar los resultados obtenidos

Archivo Implementación Desafio:

https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/Desafios/ProyectoDS_ParteI_Solis.ipynb

## Desafio Visualizaciones en Python

- Requerimientos:

    - Elegir uno de los datasets del desafío “Elección de Potenciales Datasets e importe con la librería Pandas”. Posteriormente crearán un notebook donde cargaran el archivo utilizando funciones de pandas para luego proceder a realizar 3 gráficos diferentes con Matplotlib y 3 con Seaborn. Finalmente cada gráfico será interpretado con el fin de obtener insights relevantes que permitan dar respuesta a la pregunta problema.

## Desafio Datasets con la librería Pandas

- Requerimientos:

    - Identificar 3 datasets que cumplan con las siguientes condiciones: a) al menos 2000 filas y b) al menos 15 columnas. Pueden buscar en las siguientes fuentes: GitLab, Github, Kaggle, Google Dataset Search (Si desean trabajar con un archivo propio se puede también)
    - Cargar los archivos correspondientes por medio de la librería pandas
    - Describir las variables potencialmente interesantes en cada archivo teniendo en cuenta el contexto comercial y analitico involucrado

- Archivos formato .ipynb en carpeta:
    - https://github.com/IngLuissolis/CoderHouseDataScience/blob/main/Desafios/DesafioDatasetsSolis_01.ipynb

    - https://github.com/IngLuissolis/CoderHouseDataScience/blob/main/Desafios/DesafioDatasetsSolis_02.ipynb

    - https://github.com/IngLuissolis/CoderHouseDataScience/blob/main/Desafios/DesafioDatasetsSolis_03.ipynb


- Archivos .csv en carpeta:
https://github.com/IngLuissolis/CoderHouseDataScience/tree/main/DataSets

    - DataSet 01: 2022-2023FootballPlayerStats.csv
    - DataSet 02: FootballPlayersStatsPremier2022.csv
    - DataSet 03: 2022-2023Top5FootballLeaguesPlayerStats.csv


# Descripción del Proyecto:


# Estado del Proyecto

- Completar

# Tecnologias utilizadas

- Lenguaje programación python

# Librerias utilizadas

- Completar

# Customer Homepage

Animación Gif ecommerce

# Firebase - collection orders

Imagen CartContainer

# Sitio Deployed

url

# Feedback

Any suggestion and feedback is welcome. You can message me on email

`edusolis@yahoo.com.ar`
