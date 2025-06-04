# 📅 Análisis de negocio basado en eventos
Este proyecto se centra el análisis de tres grupos de control sobre los cuales se aplicaron cambios en la interfaz de la página principal de compras para una página web mediante una prueba A/A/B. El principal objetivo consiste en determinar si los cambios aplicados generan un aumento significativo en la conversión de cada una de las etapas del embudo, para lo cual fue necesario revisar el comportamiento de cada uno de los grupos a lo largo de cada etapa del embudo y realizar pruebas estadísticas para determinar la significación de los cambios

![Analisis_embudo](https://github.com/justonenicolas/Event_based_Business_Analysis/blob/main/Embudo.JPG)

## 💡 Habilidades destacadas
* Análisis preparatorio de datos
* Análisis estadístico de datos
* Pruebas de hipótesis múltiples, paramétricas y no paramétricas 

## 🔧 Herramientas y librerías utilizadas
* Pandas
* Numpy
* Scipy

## 📊 Conclusiones generales
* Es importante mencionar que el análisis de los resultados de las pruebas indica que los datos parecen estar bien distribuídos y las muestras bien separadas, por lo cual se considera que el experimento es válido
* Al ver la distribución de los datos a lo alrgo de la prueba se pudo evidenciar que a partir del día 7 se evidenció un claro comportamiento por parte de los usuarios, por lo que se consideró relevante la información después de dicho periodo (a partir de 2019-07-31 a las 22:00)
* Tras filtrar los datos, se identificó una disminución de 2222 eventos y se desconsideraron 13 usuarios. Sin embargo, el promedio de eventos por usuario se redujo de 20 a 19 una vez filtrados los datos, lo cual indica que dichos usuarios no representaban un impacto significativo en el desarrollo de la prueba
* Tras comparar la tasa de conversión final (usuarios que realizaron compras) de los datos filtrados y sin filtrar, se evidenció que la cantidad de usuarios se reduce practicamente a la mitad para los grupos 247 y 248, pasando de 6 a 4 y 6 a 3 compras exitosas respectivamente
* Del análisis anterior se logró identificar que el grupo 246 mostró un rendimiento inferior tanto con los datos filtrados como sin filtrar (1 compra exitosa en ambos casos), incluso cuando los volumenes de tráfico en cada etapa se mantuvieron todo el tiempo dentro de los mismos rangos que los de las otras muestras. Se considera relevante poder realizar un análisis posterior para identificar los motivos de dicho resultado
* Debido a la gran cantidad de pruebas de hipótesis que se realizaron (27), se optó por utilizar un nivel de sifnificación de 0.0019, con lo cuál el nivel en conjunto de todas las pruebas será de 0.05
* Tras realizar la comparación de proporciones para eventos específicos entre datos filtrados y sin filtrar, así como la comparación de proporciones para eventos específicos entre grupos, se logró evidenciar que ninguna de las combinaciones representa una diferencia significativa entre los diferentes grupos experimentales
* Basado en lo anterior y como conclusión final, se considera que el cambio de fuentes involucrado en el grupo 248 no representa un impacto significativo en los niveles de conversión ni en los volumenes de tráfico, por lo cual se indica que si las fuentes utilizadas en este son aprobadas por los diferentes departamentos de la companía sus impactos no van a representar mayor diferencia respecto a los resultados a los producidos actualmente
