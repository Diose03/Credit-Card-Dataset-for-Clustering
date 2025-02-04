# 📊 Análisis de Segmentación de Clientes – Credit Card Dataset  

## 🎯 Objetivo  
Realizar un análisis de segmentación de clientes aplicando técnicas estadísticas, algoritmos de machine learning y heurísticas. Se busca identificar patrones en los datos y definir estrategias de marketing.  

## 📌 Dataset: Credit Card Dataset for Clustering  
- **Fuente**: Dataset de Kaggle con9000 titulares de tarjetas de crédito activos en los últimos 6 meses.  
- **Variables**: 18 características relacionadas con el uso de la tarjeta de crédito.
- **Más info: [Accede aquí](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata/data).

## 📑 Diccionario de Datos  
Algunas de las variables clave del dataset incluyen:  
- **BALANCE**: Saldo restante en la tarjeta.  
- **PURCHASES**: Monto total de compras realizadas.  
- **CREDIT_LIMIT**: Límite de crédito del usuario.  
- **PAYMENTS**: Monto total de pagos realizados.  
- **TENURE**: Tiempo de servicio del usuario con la tarjeta.  

## 🛠️ Preprocesamiento de Datos  
- Eliminación de la columna **CUST_ID** (no aporta valor al análisis).  
- Manejo de valores nulos en **CREDIT_LIMIT** y **MINIMUM_PAYMENTS** utilizando la mediana.  
- Detección y eliminación de **outliers** con el método del **rango intercuartil (IQR)**.  
- Reducción del dataset de **8950 a 5525 registros**.  
- Normalización de los datos para mejorar la eficiencia de los algoritmos.  

## 🔬 Análisis de Componentes Principales (PCA)  
- Aplicación de **PCA** para reducir la dimensionalidad y mejorar la interpretación.  
- **Primer componente (35.09%)** + **Segundo componente (26.86%)** = **61.95% de la varianza total**.  
- Visualización de los datos proyectados en dos dimensiones.  

## 🔢 Segmentación con K-Means  
- Determinación del número óptimo de **clusters** con el **Método del Codo** y el **Coeficiente de Silueta**.  
- Se seleccionó **K = 3** como el número óptimo de clusters.  
- Visualización de los clusters en el espacio PCA.  

## 🧬 Algoritmo Genético  
- Implementación de **algoritmos genéticos** para optimizar la segmentación de clientes.  
- Evaluación con **distancia Euclidiana y Manhattan**.  
- La **distancia Euclidiana** mostró mejor rendimiento y coherencia en la segmentación.  

## 🔍 Análisis de Resultados  
- **Matriz de correlación** para identificar relaciones entre variables.  
- Visualización de los clusters segmentados.  
- Resumen estadístico de los clusters con **media, desviación estándar, mínimo y máximo**.  
- Interpretación de cada grupo según su comportamiento financiero.  

## 📊 Conclusión  
<p align="justify">
La segmentación de clientes permite desarrollar estrategias de marketing más efectivas, optimizando la gestión del crédito y ofreciendo mejores servicios personalizados.  
En base a los segmentos obtenidos de nuestro análisis de datos, con el objetivo de definir una estrategia de marketing, se sugiere lo siguiente:<br>  
<strong>○ Cluster 0:</strong> Se recomienda una estrategia de alto valor y promociones exclusivas para atraer a clientes con potencial pero menos activos.<br>
<strong>○ Cluster 1:</strong> Se sugieren incentivos para aumentar el uso del crédito y la oferta de productos complementarios para fomentar aún más su consumo.<br>  
<strong>○ Cluster 2:</strong> Se recomienda ofrecer promociones de bajo riesgo y estrategias de fidelización para mantener a los clientes comprometidos sin asumir riesgos elevados.  
</p>



