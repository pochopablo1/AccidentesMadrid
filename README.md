# AccidentesMadrid

Predicción de accidentes de tráfico en Madrid (2012-2018)
Este proyecto se enfoca en el análisis de datos de accidentes de tráfico ocurridos en la ciudad de Madrid entre 2012 y 2018, con el objetivo principal de desarrollar un modelo predictivo para estimar el número de accidentes futuros.

El análisis completo y el desarrollo del modelo se realizaron utilizando Python y se documentan en el informe ejecutivo adjunto. 


Link al código: https://colab.research.google.com/drive/1SOllyj7BAsbIKzgUwwSy4aEFgntrqLhg?usp=sharing 

📜 Descripción del proyecto
El análisis utiliza un conjunto de datos del portal de datos abiertos del Ayuntamiento de Madrid, que incluye únicamente los accidentes con heridos o daños al patrimonio municipal. A través de técnicas de limpieza, análisis exploratorio y modelado de series temporales, se busca predecir la cantidad de accidentes en meses futuros. 


📊 Análisis descriptivo: 
Hallazgos principales
El análisis exploratorio de los datos reveló patrones temporales, geográficos y de tipología de accidentes muy claros. 

Patrones temporales: Los viernes son los días con mayor número de accidentes, mientras que los domingos son los de menor incidencia. El rango horario de 14:00 a 15:00 horas concentra la mayor frecuencia. 

Distribución geográfica: El distrito de Salamanca es el que registra la mayor cantidad de accidentes, seguido por Chamartín y Centro. 

Tipología de accidentes: La colisión doble es, por mucho, el tipo de accidente más frecuente. 

Perfil de involucrados: Los hombres son los conductores más comúnmente implicados en accidentes. 

Visualizaciones clave
1. Accidentes por día de la semana: Se observa un pico claro los viernes y un valle los domingos. 

2. Accidentes por distrito: Muestra la alta incidencia en distritos céntricos y de alta actividad como Salamanca. 

3. Accidentes por tipo: La colisión doble domina las estadísticas, indicando que es el suceso más común en las calles de Madrid. 

🧠 Metodología Predictiva
Para la predicción se optó por un modelo de series temporales, específicamente un modelo ARIMA (Autoregressive Integrated Moving Average). 

División de datos: El conjunto de datos se dividió en un set de entrenamiento (hasta septiembre de 2018) y uno de prueba (desde octubre de 2018 en adelante). 

Ajuste del modelo: Se utilizó la función auto_arima para encontrar los parámetros óptimos del modelo, resultando en un ARIMA(2, 1, 2). 

Evaluación: El modelo se evaluó con el conjunto de prueba, obteniendo un Error Cuadrático Medio (RMSE) de 252.29. 


🚀 Próximos Pasos
Para mejorar la precisión y utilidad del modelo, se proponen los siguientes pasos: 

Ajustar parámetros ARIMA: Explorar manualmente diferentes configuraciones (p, d, q). 


Incorporar estacionalidad: Añadir componentes estacionales al modelo para capturar patrones anuales. 


Usar variables exógenas: Enriquecer el modelo con datos climáticos, de tráfico o sobre eventos especiales (festivos, etc.). 


Explorar modelos alternativos: Evaluar el rendimiento de otros algoritmos como XGBoost. 


Crear un sistema de alerta: Integrar el modelo final en un sistema de alerta temprana para la toma de decisiones preventivas. 

👨‍💻 Autor

Pablo Santilli 

📚 Referencias

IBM - Algoritmos de Machine Learning 


MIOTI - Deep Learning y Seguridad Vial 


Public Health, Columbia University - Metodología Box-Jenkins 
