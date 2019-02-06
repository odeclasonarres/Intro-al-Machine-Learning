### **MOD1. Introducción al Machine Learning?**

### **MOD2. Nuestros datos. ¿Están preparados para el Machine Learning?**

##### 1. Tipos de datos útiles y su formato
Los datos tienen que estar en un formato correcto(ML ready). Necesario uniformizar datos en formatos tabulados(csv), una fila una instancia, una columna una propiedad.

Utilizamos BigML.com
  * Tipos de datos:
    * Numeric
    * Categorical
    * Text
    * Items
    * Datetime


Preparación de datos para AA:
  * Asegurar que los campos tienen el tipo adecuado.
  * Asegurar que sus valores se interpretan correctamente.

##### 2. Análisis de datos antes del modelado
Una vez vez verificados formatos y atributos se crea un dataset, que proporciona un resumen de los datos de la tabla; campo a campo desglosa:
 * Cantidad de instancias,
 * Cantidad de instancias con valor,
 * Cantidad de instancias sin valor,
 * Cantidad de instancias con valores erroneos
 * Distribución de datos(frecuencia) a través de histograma.
 * Los campos numéricos tienen un desplegable con estadísticas(mínimo, máximo, media....)

 ¿Qué información aporta?
  * Campos id(números consecutivos) ---> Distribuciones que no son útiles para el aprendizaje(se señala con signo de exclamación), se excluirá.
  * Los campos fecha se descomponen para obtener valor

¿Cómo aprovechamos la información? Feature engineering(ingeniería de atributos)
  * Cada campo del dataset puede ser útil o no en el aprendizaje
    * Predictor: campo útil para predecir
      * Se pueden añadir al dataset basándonos en campos existentes.
      * Se pueden modificar un campo ya existente(p.ejem agrupar edades para clasificar en jóvenes, mayores....)

### **Mod3. ML, aprendizaje supervisado**
##### **1. Clasificación y regresión: árboles de decisión**
**Árbol de decisión**: Modelo para descubrir los patrones que hay en nuestros datos y poder predecir resultados cuando tenemos todos los datos. Dataset+campo objetivo.

**¿Cómo se construye, qué obtenemos?**
* Encontrando un campo objetivo
* 1-clic-model: Extrae los platrones existentes, **entrena el modelo**. Nodo raíz y nodos terminales.
* Camino de nodo raíz a terminal: forman un patrón que define una predicción. Cada predicción tiene una fiabilidad en base al modelo(probabilidad pura). Podemos filtrar en función de la confianza y soporte o en base a un valor concreto.
* Predicción del valor del campo objetivo para un nuevo caso.
* Preguntas determinantes para la predicción y su importancia relativa.
* Cada campo del modelo es un predictor.


**Bondad de un modelo** = confianza+evaluación *(casos que no se hayan usado en el entrenamiento)*


##### **2. Predicción y evaluación**
¿Cómo medir la calidad de un modelo de aprendizaje supervisado? Evaluación: comparar las predicciones hechas para casos de los que ya sabemos el resultado *(pero que no han formado parte del entrenamiento)*.

* Modelo útil: adaptado pero general con otros casos.
* Modelo demasiado adaptado: no generaliza.


* ¿Cómo contrastar predicciones? Métricas de evaluación:
  * **Exactitud** *(accuracy)*: Total de aciertos, total de predicciones.
  * **Precisión**:
  * **Exhaustividad**:
  * **Combinación**:


* Errores de predicción--->Genera un coste--->En función del coste y del tipo de problema nos quedaremos con un modelo u otro.

### **Mod4. ML, aprendizaje no supervisado**
El objetivo de este módulo es explicar mediante ejemplos algunas de las soluciones del Machine Learning a problemas de aprendizaje no supervisado. Se tratarán los problemas de segmentación (clustering), detección de anomalías y descubrimiento de asociaciones.

##### **1. Segmentación y clusters**
**Clustering**: Organizar automáticamente datos en grupos de instancias similares entre ellas y distintas de las demás. 
  * Agrupa datos con algoritmo G-means

##### **2. Detección de anomalías**


##### **3. Reglas de asociación**
