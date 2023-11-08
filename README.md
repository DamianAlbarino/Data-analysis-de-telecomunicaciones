<p align='center'>
<img src ="https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png">
<p>

<h1 align='center'><b>PROYECTO INDIVIDUAL Nº2</b></h1>

# <h1 align="center">**`Telecomunicaciones`**</h1>

## **Descripción del problema -contexto y rol a desarrollar-**

### **Contexto**

Las telecomunicaciones se refieren a la transmisión de información a través de medios electrónicos, como la telefonía, la televisión, la radio y, más recientemente, el internet. Estos medios de comunicación permiten la transmisión de información entre personas, organizaciones y dispositivos a largas distancias.

El internet, por su parte, es una red global de computadoras interconectadas que permite el intercambio de información en tiempo real. Desde su creación, ha tenido un impacto significativo en la vida de las personas, transformando la manera en que nos comunicamos, trabajamos, aprendemos y nos entretenemos.

La industria de las telecomunicaciones ha jugado un papel vital en nuestra sociedad, facilitando la información a escala internacional y permitiendo la comunicación continua incluso en medio de una pandemia mundial. La transferencia de datos y comunicación se realiza en su mayoría a través de internet, líneas telefónicas fijas, telefonía móvil, y en casi cualquier lugar del mundo. 

En comparación con la media mundial, Argentina está a la vanguardia en el desarrollo de las telecomunicaciones, teniendo para el 2020 un total de [62,12 millones de conexiones](https://www.datosmundial.com/america/argentina/telecomunicacion.php). 


### **Rol a desarrollar**

En este contexto, una empresa prestadora de servicios de telecomunicaciones le encarga a usted la realización de un **análisis** completo que permita reconocer el comportamiento de este sector a nivel nacional. Considere que la principal actividad de la empresa es brindar **acceso a internet**, pero también es importante considerar el comportamiento asociado al resto de los servicios de comunicación, con el fin de orientar a la empresa en brindar una buena calidad de sus servicios, identificar oportunidades de crecimiento y poder plantear soluciones personalizadas a sus posibles clientes.

# **Trabajo realizado**

## `EDA` (Exploratory Data Analysis)

En este proyecto, se ha realizado un análisis detallado de varios datasets seleccionados, que incluyen los siguientes archivos:

- `1_Internet_Penetracion.xlsx`
- `2_Internet_BAF.xlsx`
- `3_Internet_Accesos-por-tecnologia.xlsx`
- `4_historico_velocidad_internet.xlsx`

El análisis completo de estos datasets se encuentra documentado en el archivo `EDA.ipynb`, donde se detallan las exploraciones, transformaciones y hallazgos clave de los datos.

Además, como parte de la fase de preparación para la creación del dashboard, se han generado diversos gráficos con el objetivo de comprender a fondo la información contenida en los datasets. Estos gráficos desempeñan un papel fundamental al proporcionar un contexto visual que facilitará la interpretación de los indicadores clave de rendimiento (KPIs) en el dashboard final.

### Resumen del analisis del EDA:

Al observar el dataset `1_Internet_Penetracion.xlsx` podemos ver que contiene el acceso a internet en diferentes provincias cada 100 hogares de Argentina durante el año 2014 hasta el 2022 y separados por trimestres del año. 

![Grafico de lineas acceso cada 100 hogares](https://github.com/DamianAlbarino/Proyecto-Individual-Nro-2/blob/main/img/GraficoLineas100H.png?raw=true)

Pudimos ver que el acceso a internet cada 100 hogares hay una diferencia muy grande con capital federal y el resto de las provincias, ya desde un principio capital federal lidera esta metrica. Esto puede estar influenciadas por una serie de factores, como inversiones en infraestructura, población, políticas gubernamentales, demanda de servicios, avances tecnológicos y eventos económicos y sociales.

![Grafico de barras prov x prov acceso cada 100 hogares](https://github.com/DamianAlbarino/Proyecto-Individual-Nro-2/blob/main/img/provinciaXprovincia100H.png?raw=true)

Al analizar provincia por provincia, podemos identificar saltos significativos en el gráfico de barras, lo cual es de particular interés. Estos saltos representan áreas de oportunidad que merecen un estudio más detallado. Por ejemplo, en provincias como San Luis (2018 Trim 2 al Trim 3), La Rioja (2021 Trim 1 al Trim 2), Jujuy (2018 Trim 3 al Trim 4) y Tierra del fuego (2021 Trim 2 al Trim 3), entre otros, observamos un incremento notorio en la métrica de acceso a Internet por cada 100 hogares.

El dataset `2_Internet_BAF.xlsx` muestra información recopilada a lo largo de varios años y trimestres en Argentina sobre la conectividad a Internet en diversas provincias del país.

![Grafico de barras Banda ancha y Dial Up](https://github.com/DamianAlbarino/Proyecto-Individual-Nro-2/blob/main/img/GraficoBarrasDialUpBandaAncha.png?raw=true)

Existe una disparidad notoria en la cantidad de usuarios entre la banda ancha y Dial-up, y esta brecha se debe principalmente a las marcadas diferencias en la velocidad de conexión entre estos dos tipos de servicios. La banda ancha representa una tecnología de conexión a Internet significativamente más rápida, estable y costosa en comparación con el Dial-up. El Dial-up es una alternativa más económica, pero a expensas de velocidades de conexión considerablemente más lentas y una menor estabilidad en la conexión.

Es importante destacar que, a medida que transcurre el tiempo, se ha observado una disminución gradual en la utilización del servicio de conexión Dial-up

El dataset `3_Internet_Accesos-por-tecnologia.xlsx` proporciona información sobre el tipo de tecnologia para el acceso a Internet en Argentina durante 2014-2022 separados en trimestres.

![Grafico de lineas acceso por tecnologia](https://github.com/DamianAlbarino/Proyecto-Individual-Nro-2/blob/main/img/graficoLineasAccesoXTec.png?raw=true)

El gráfico de lineas refleja cómo el ADSL muestra una disminución notable, en línea con la tendencia de disminución del Dial Up, mientras que la Banda Ancha y el Cablemódem como la fibra óptica están en aumento, lo que refleja la creciente demanda de velocidades más altas.
La fibra óptica se perfila como el estándar del futuro, por lo que es posible prever que en breve también comenzará a disminuir la métrica relacionada con el cablemódem a medida que se realice la transición hacia la fibra óptica.

El dataset `4_historico_velocidad_internet.xlsx`contiene información sobre la velocidad promedio de descarga de conexiones a Internet en diferentes provincias de Argentina a lo largo del 2014 al 2022 y sus respectivos trimestres.

![Grafico de lineas Mbps](https://github.com/DamianAlbarino/Proyecto-Individual-Nro-2/blob/main/img/GraficoLineasMbps.png?raw=true)

Se observa una variación notoria en la velocidad de Internet en diferentes provincias a lo largo de este período.
A partir del año 2018, algunas provincias experimentaron un aumento significativo en sus velocidades de conexión, lo que puede indicar mejoras significativas en la infraestructura de Internet.
Por otro lado, algunas provincias muestran un crecimiento más lento en la velocidad de Internet durante este período, como Chubut que han mantenido una velocidad de Internet relativamente constante sin experimentar un crecimiento significativo en comparación con el resto de las provincias.

![Grafico de barras 20 Mbps](https://github.com/DamianAlbarino/Proyecto-Individual-Nro-2/blob/main/img/MenorA20Mbps.png?raw=true)

Observamos que en el cierre de 2022, solo unas pocas provincias aún mantienen velocidades promedio por debajo de 20 Mbps. Estas provincias presentan una notable oportunidad de crecimiento en el mercado, aprovechando la tendencia tecnológica actual a nivel mundial. La demanda de conexiones de alta velocidad es evidente, y estas áreas podrían beneficiarse significativamente de inversiones en infraestructura y servicios de Internet para satisfacer las necesidades en constante evolución de la sociedad moderna.

## `Dashboard`

Este dashboard ha sido creado utilizando Power BI y está diseñado para proporcionar una experiencia interactiva para el seguimiento y análisis de datos clave.

Visualización del Dashboard

Puedes acceder y explorar el dashboard desde el repositorio. El archivo del proyecto de Power BI se encuentra en el repositorio con el nombre `"Proyecto Individual.pbix"`. Para visualizarlo, sigue estos pasos:

1. Ve al archivo `"Proyecto Individual.pbix"` en el repositorio.
2. Haz clic en el archivo para abrirlo en Power BI.
3. Explora las diferentes visualizaciones y utiliza las funciones interactivas para analizar los datos.

## `KPIs`

- *`Aumentar en un 2% el acceso al servicio de internet para el próximo trimestre, cada 100.`*

Formula utilizada =  $`KPI = ((Nuevo Acceso - Acceso Actual) / Acceso Actual) * 100`$

Donde:
- "Nuevo Acceso" se refiere al número de hogares con acceso a Internet después del próximo trimestre.
- "Acceso Actual" se refiere al número de hogares con acceso a Internet en el trimestre actual.

Ejemplo para el 2023 Trim. 1: ![KPI Acceso 100 hogares](https://github.com/DamianAlbarino/Proyecto-Individual-Nro-2/blob/main/img/KPIAcceso100H.png?raw=true)

- *`Aumentar en un 2% las conexiones por fibra óptica Ejemplo para el próximo trimestre.`*

Formula utilizada =  $`KPI = ((Nuevos Usuarios - Usuarios Actuales) / Usuarios Actuales) * 100`$

Donde:
- "Nuevo Usuarios" se refiere a la cantidad de usuarios de fibra óptica después del próximo trimestre.
- "Usuarios Actuales" se refiere a la cantidad de usuario actual de fibra óptica del trimestre actual.

Ejemplo para el 2023 Trim. 1: ![KPI Fibra optica](https://github.com/DamianAlbarino/Proyecto-Individual-Nro-2/blob/main/img/KPIFibraOptica.png?raw=true)

- *`Reducir en un 5% el acceso a internet por dial up.`*

Formula utilizada =  $`KPI = ((Conexiones nuevas - Conexiones actuales) / Conexiones actuales) * 100`$

Donde:
- "Conexiones nuevas" se refiere al número conexions a internet por dial up después del próximo trimestre.
- "Conexiones actuales" se refiere al número conexions a internet por dial up en el trimestre actual.

Ejemplo para el 2023 Trim. 1: ![KPI Dial up](https://github.com/DamianAlbarino/Proyecto-Individual-Nro-2/blob/main/img/KPIDialUp.png?raw=true)

- *`Mejorar un 10% el promedio de Mbps en las provincias con promedio menor a 20 Mbps.`*

Formula utilizada =  $`KPI = ((Mbps nuevos - Mbps actual) / Mbps actual) * 100`$

Donde:
- "Mbps nuevos" se refiere a la cantidad de mbps después del próximo trimestre.
- "Mbps actual" se refiere a la cantidad de mbps en el trimestre actual.

Ejemplo para el 2023 Trim. 1: ![KPI Mbps](https://github.com/DamianAlbarino/Proyecto-Individual-Nro-2/blob/main/img/KPIProvincias.png?raw=true)
