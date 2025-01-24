# Análisis de Calidad de Vinos usando Minería de Datos

## Descripción del Proyecto
Este proyecto tiene como objetivo analizar la calidad de vinos basada en sus propiedades químicas utilizando técnicas de minería de datos. Se implementó un modelo de Árbol de Decisión para predecir la calidad del vino y se generaron visualizaciones para comprender mejor los resultados y las características del dataset.

El repositorio incluye el código desarrollado, gráficos generados y un análisis detallado, lo que lo convierte en un recurso valioso para aprender sobre minería de datos y aprendizaje automático.

---

## Dataset
### Descripción
El dataset utilizado proviene de un conjunto de datos sobre vinos, donde cada entrada representa las propiedades químicas de un tipo de vino. La variable objetivo es **`quality`**, que indica la calidad del vino en una escala del 0 al 10.

### Atributos del Dataset
- **fixed acidity**: Acidez fija.
- **volatile acidity**: Acidez volátil.
- **citric acid**: Contenido de ácido cítrico.
- **residual sugar**: Azúcares residuales.
- **chlorides**: Cloruros.
- **free sulfur dioxide**: Dioxido de azufre libre.
- **total sulfur dioxide**: Dioxido de azufre total.
- **density**: Densidad.
- **pH**: Nivel de pH.
- **sulphates**: Sulfatos.
- **alcohol**: Contenido de alcohol.
- **quality**: Calidad del vino (variable objetivo).

El dataset está en formato `.csv` y se encuentra en la carpeta `data/`.

---

## Código Desarrollado
El código desarrollado se encuentra en el archivo `src/decision_tree_analysis.py`. Los pasos principales incluyen:

1. **Carga de Datos**: Se utiliza Pandas para cargar y explorar el dataset.
2. **Preparación del Dataset**:
   - Separación de las características (X) y la variable objetivo (y).
   - División del dataset en conjuntos de entrenamiento y prueba (80% - 20%).
3. **Entrenamiento del Modelo**:
   - Implementación de un modelo de Árbol de Decisión con Scikit-learn.
   - Ajuste del modelo utilizando los datos de entrenamiento.
4. **Evaluación del Modelo**:
   - Generación de predicciones con el conjunto de prueba.
   - Cálculo de métricas como `accuracy` y matriz de confusión.
5. **Visualización**:
   - Gráficos para la matriz de confusión, importancia de las características y distribución de la variable `quality`.

Para ejecutar el código, asegúrate de instalar las dependencias especificadas en el archivo `requirements.txt`.

---

## Resultados y Visualizaciones

### 1. **Matriz de Confusión**
La matriz de confusión muestra el desempeño del modelo al comparar las predicciones con los valores reales de calidad del vino.

![Matriz de Confusión](https://github.com/daniel-alegria-z/Calidad-de-Vinos/blob/main/visuales/matriz_confusion.png)

### 2. **Importancia de las Características**
Este gráfico destaca las características más influyentes en el modelo de Árbol de Decisión.

![Importancia de las Características](../visuales/caracteristicas.png)

### 3. **Distribución de la Calidad del Vino**
La distribución de la variable `quality` permite observar la cantidad de ejemplos en cada clase.

![Distribución de la Calidad del Vino](../visuales/distribucion_calidad.png)

---

## Estructura del Repositorio
```
├── datos/
│   └── Calidad_de_vinos.csv  # Dataset utilizado
├── src/
│   └── decision_tree_analysis.py  # Código principal
├── visuales/
│   ├── matriz_confusion.png  # Gráfico de matriz de confusión
│   ├── caracteristicas.png  # Gráfico de importancia de características
│   └── distribucion_calidad.png  # Gráfico de distribución de calidad
├── README.md  # Descripción del proyecto
├── requirements.txt  # Dependencias necesarias
```

---

## Dependencias
Para ejecutar el proyecto, instala las siguientes librerías de Python:

```
pandas
scikit-learn
matplotlib
seaborn
```
Puedes instalarlas ejecutando:
```
pip install -r requirements.txt
```

---

## Contribuciones
Las contribuciones son bienvenidas. Si deseas mejorar el proyecto o agregar nuevas funcionalidades, no dudes en hacer un fork y enviar un pull request.

---

## Licencia
Este proyecto está licenciado bajo la licencia MIT. Consulta el archivo `LICENSE` para obtener más información.

---

## Autor
Creado por Daniel Esteban Alegría Zamora como un ejercicio educativo en minería de datos. Si tienes preguntas o sugerencias, no dudes en contactarme.

