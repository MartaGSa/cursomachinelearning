# cursomachinelearning
Ejercicios realizados en el curso de Machine Learning.
Hemos utilizado el lenguaje Python.
## Ejercicio 'SpaceX 2 EDA':
  - Hemos hecho un análisis de datos exploratorio en la búsqueda de patrones en los datos 
  y así determinar qué valores debemos usar para realizar predicciones en un futuro.
  - Hemos querido predecir la probabilidad de éxito basándonos en ciertas categorías.
  - Para ello, hemos: 
    1. Calculado el número de lanzamientos en cada plataforma.
    2. Calculado el número de lanzamientos para cada órbita.
    3. Calculado el número de diferentes resultados de aterrizaje, distinguiendo los exitosos de los fallidos.
## Ejercicio 'Prophet, Predecir el valor de Bitcoin':
  - Práctica para predecir del valor de Bitcoin.
  - Para ello, hemos:
    1.  Volcado y descargado el histórico de datos de Bitcoin desde Yahoo Finance.
    2. Validado que no hay datos vacíos.
    3. Filtrado el dataframe para quedarnos con las columnas "Date" y "Open" (que son las que nos interesan).
    4. Creado un diccionario con los valores que espera el Prophet (X e Y).
    5. Transformado en fecha la columna "Date" sin zona horaria para que pueda trabajar correctamente el Prophet.
    6. Creado la gráfica del precio de apertura.
    7. Una vez visualizada la gráfica de datos, hemos inicializado el Prophet y lo hemos entrenado pasándole el dataframe. 
    8. Generado un dataframe con los días que tenemos y los 365 días siguientes (que queremos predecir).
## Ejercicio 'Introducción a Machine Learning con Scikit-Learn':
- Hemos integrado los datos en un dataframe de Pandas para aplicar las técnicas de data-wrangling.
- Dividimos nuestros datos en dos grupos: Train (los datos desde los que aprender) y Test (el resultado que tiene que dar dichos datos), con la función de Scikit-learn.
- Hemos utilizado el modelo KNearestNeighbor, del que hemos creado una instancia y la hemos entrenado.
- Utilizando los conjuntos de entrenamiento y test anteriores, hemos entrenado un modelo de regresión lineal y hemos realizado la predicción del conjunto test y 
  representado la predicción gráficamente mediante un ScatterPlot. 
- Hemos mejorado la predicción corrigiendo la escala. Para ello: hemos realizado un proceso de estandarización de datos mediante el preprocessing, 
  que hemos automatizado mediante una pipeline.
- Para optimizarlo más, hemos aplicado un escalado de estandarización a un modelo de regresión.
- Hemos comparado los datos obtenidos con otro entrenamiento del modelo, esta vez con todos los datos para ver si es capaz de realizar mejores predicciones que el anterior.
- Hemos modificado un hyperparámetro para ver lo que sucede con los datos en este caso con más detalle. 
- Hemos introducido una nueva herramienta de Scikit Learn: GridSearchCV, para dividir test y train, buscar el mejor hiperparámetro y entrenar la red con dicho parámetro.
- Para ello, hemos:
  1. Sacado un listado de los hiperparámetros con los que podíamos trabajar y hemos elegido los que íbamos a optimizar.
  2. Utilizado el Cross Validation para poder probar diferentes hiperparámetros, entrenar el modelo y asegurar que la división entre train y test no altera el modelo.
  3. Aplicado el método de cross validation a la regresión Ridge.
  4. Realizado una gráfica que presente las predicciones del modelo mediante KNN Regresion y Ridge Regresion.
