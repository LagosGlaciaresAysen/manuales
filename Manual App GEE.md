# <p align="center">Manual de usuario para aplicación de Earth Engine</p>
## <p align="center">Identificación de lagos glaciares y visualización de variaciones superficiales históricas</p>
<p align="justify">El siguiente manual se describe el uso de la aplicación realizada en ambiente de <em>Google Earth Engine Apps. </em>Esta aplicación tiene como objetivo graficar series de tiempo del cambio de la superficie de lagos glaciares en Chile y facilitar la descarga de datos vectoriales y csv. La figura 1 muestra la interfaz gráfica.</p>
<p>&nbsp;</p>

<p align="center"><img src="https://user-images.githubusercontent.com/101720220/204846409-32fb2d5c-2534-4299-8139-1b52bdff13c3.png" width="800"
   height="400"></p>

**Figura 1:** Interfaz gráfica de la aplicación desarrollada para mapear y monitorear lagos glaciares.
<p>&nbsp;</p>
<p align="justify">En la parte izquierda de la aplicación se detallan algunas instrucciones para el usuario (Figura 2). Luego se presenta la selección de variables que se describen a continuación.</p>
<ol>
<li>Fecha de inicio: selección de fecha en que comienza el análisis.</li>
<li>Fecha de término: selección de fecha en que termina el análisis</li>
<li>Porcentaje de nubosidad: porcentaje de la imagen que se encuentra cubierta por nubosidad. En caso de la colección Landsat se encuentra determinada por la propiedad &lsquo;<em>cloud_cover&rsquo;, </em>y en caso de Sentinel 2 por &lsquo;<em>cloudy_pixel_percentage&rsquo;. </em>A la colección Sentinel 1 no le afecta esta variable dado que corresponde a imágenes radar.</li>
</ol>
<p align="justify">Se sugiere que para Patagónia se ocupe valores de porcentaje de nubosidad más altos (⁓ 10%), mientras que para Chile central valores más bajos (⁓5%). Esto permitirá tener mayor disponibilidad de imágenes en Patagonia y reducir el n&uacute;mero de imágenes en la zona central&nbsp; para agilizar los tiempos de computo y descarga de datos.</p>
<ol start="4">
<li>Selección de colección: Elección de la colección de imágenes satelitales o de radar que se tiene como objetivo para el análisis. Al seleccionar cualquiera de las 3 opciones automáticamente se desplegarán los resultados en la parte derecha. Si se requiere realizar otro análisis, simplemente se presiona otra vez ese botón y se mostrarán los nuevos resultados.</li>
</ol>
<p align="justify">Descarga de shapefile: una vez seleccionada la colección, se podrá descargar el shapefile resultante de la delimitación de lagos glaciares seleccionado del periodo elegido. Este cuenta con una columna indicando d&iacute;a, mes y a&ntilde;o de la imagen además del área de cada pol&iacute;gono en km<sup>2</sup>.&nbsp;</p>

<p align="center">  <img width="164" alt="Imagen2" src="https://user-images.githubusercontent.com/101720220/204847431-b0cdcab8-63c9-4fb5-8620-ab93848dff49.png"  height="400"></p>

**Figura 2:** Pesta&ntilde;a mostrando las variables que debe seleccionar el usuario para realizar el mapeo y análisis de variaciones históricas de lagos glaciares. Nótese que la &uacute;ltima opción (Descargar resultado Landsat) sólo se activa y aparece cuando se ha ejecutado la herramienta. El nombre de ese hiperv&iacute;nculo cambia dependiendo de la colección de imágenes seleccionada.

<p align="justify">En la parte central de la interfaz se encuentra desplegado el mapa base. Se puede seleccionar el mapa base de Google o el mapa base satelital de Google. Estas opciones se encuentran ubicadas en la parte superior derecha del mapa (Figura 3). En esta pantalla el usuario debe delimitar el pol&iacute;gono de área de estudio -lago glaciar- que quiera analizar. Este pol&iacute;gono se dibuja con las herramientas de geometr&iacute;a ubicadas en la parte superior izquierda. El área seleccionada puede ser un rectángulo o pol&iacute;gono irregular. En esta pantalla se superpone automáticamente la imagen más reciente de la colección analizada.</p>

<p align="center"><img src="https://user-images.githubusercontent.com/101720220/204865983-2e2ab6ef-4f68-47ea-8ba5-5fd32c386b52.png" width="736"
   height="665"></p>
   
**Figura 3:** Mapa base e interfaz para delimitar lagos glaciares para el análisis. Se despliega la imagen más reciente de la colección escogida (Landsat, Sentinel 1 o Sentinel 2).

<p align="justify">Por &uacute;ltimo, en la parte en la parte derecha de la interfaz, se encuentran los resultados del análisis. En primer lugar, se visualizará un <em>GIF</em> de las imágenes ocupadas por la clasificación, con la opción de poder descargar a un disco local el archivo GIF de la animación. Luego se mostrarán los gráficos de cálculo de área a través de tiempo del lago glaciar seleccionado y la tasa de cambio de área (km<sup>2</sup>) entre imágenes sucesivas (figura 4)</p>

<p align="center"><img src="https://user-images.githubusercontent.com/101720220/204866237-4f099950-87df-48a8-92d3-6d8f002cf8cb.png" width="264"
   height="685"></p>

**Figura 4:** Ventana&nbsp; de&nbsp; resultados mostrando en la parte superior animación con las imágenes seleccionadas y en la parte inferior los gráficos de variación histórica y tasa de cambio de la superficie de los lagos.

<p align="justify">Los gráficos son interactivos y permiten inspeccionar la fecha y área estimada en cada imagen (e.i. en cada punto del gráfico). Los gráficos tienen una pesta&ntilde;a en la parte superior derecha. Seleccionando esa pesta&ntilde;a se despliega una nueva ventana con el gráfico seleccionado (Figura 5). En esta ventana se da la opción de descargar los datos del gráfico en formato csv, o decargar el gráfico mismo en formatos SVG y PNG.</p>

<p align="center"><img src="https://user-images.githubusercontent.com/101720220/204867443-e271dc3c-7de6-437c-a8d0-69e85557daf4.png" width="334"
   height="274"></p>


**Figura 5:** Gráfico de cambio de superficie de lago glaciar seleccionado. En la parte superior derecha se muestra las opciones de descarga de datos.
