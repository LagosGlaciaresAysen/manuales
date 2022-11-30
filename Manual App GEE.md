# <p style="text-align: center;">Manual de usuario para aplicación de Earth Engine</p>
## <p>Identificaci&oacute;n de lagos glaciares y visualización de variaciones superficiales históricas</p>
<p>El siguiente manual se describe el uso de la aplicación realizada en ambiente de <em>Google Earth Engine Apps. </em>Esta aplicación tiene como objetivo graficar series de tiempo del cambio de la superficie de lagos glaciares en Chile y facilitar la descarga de datos vectoriales y csv. La figura 1 muestra la interfaz gr&aacute;fica.</p>
<p>&nbsp;</p>

<p><img src="https://user-images.githubusercontent.com/101720220/204846409-32fb2d5c-2534-4299-8139-1b52bdff13c3.png" width="800"
   height="400"></p>


<p>Figura 1: Interfaz gr&aacute;fica de la aplicaci&oacute;n desarrollada para mapear y monitorear lagos glaciares</p>
<p>&nbsp;</p>
<p>En la parte izquierda de la aplicaci&oacute;n se detallan algunas instrucciones para el usuario (Figura 2). Luego se presenta la selecci&oacute;n de variables que se describen a continuaci&oacute;n.</p>
<ol>
<li>Fecha de inicio: selecci&oacute;n de fecha en que comienza el an&aacute;lisis.</li>
<li>Fecha de t&eacute;rmino: selecci&oacute;n de fecha en que termina el an&aacute;lisis</li>
<li>Porcentaje de nubosidad: porcentaje de la imagen que se encuentra cubierta por nubosidad. En caso de la colecci&oacute;n Landsat se encuentra determinada por la propiedad &lsquo;<em>cloud_cover&rsquo;, </em>y en caso de Sentinel 2 por &lsquo;<em>cloudy_pixel_percentage&rsquo;. </em>A la colecci&oacute;n Sentinel 1 no le afecta esta variable dado que corresponde a im&aacute;genes radar.</li>
</ol>
<p>Se sugiere que para Patag&oacute;nia se ocupe valores de porcentaje de nubosidad m&aacute;s altos (⁓ 10%), mientras que para Chile central valores m&aacute;s bajos (⁓5%). Esto permitir&aacute; tener mayor disponibilidad de im&aacute;genes en Patagonia y reducir el n&uacute;mero de im&aacute;genes en la zona central&nbsp; para agilizar los tiempos de computo y descarga de datos.</p>
<ol start="4">
<li>Selecci&oacute;n de colecci&oacute;n: Elecci&oacute;n de la colecci&oacute;n de im&aacute;genes satelitales o de radar que se tiene como objetivo para el an&aacute;lisis. Al seleccionar cualquiera de las 3 opciones autom&aacute;ticamente se desplegar&aacute;n los resultados en la parte derecha. Si se requiere realizar otro an&aacute;lisis, simplemente se presiona otra vez ese bot&oacute;n y se mostrar&aacute;n los nuevos resultados.</li>
</ol>
<p>&nbsp;Descarga de shapefile: una vez seleccionada la colecci&oacute;n, se podr&aacute; descargar el shapefile resultante de la delimitaci&oacute;n de lagos glaciares seleccionado del periodo elegido. Este cuenta con una columna indicando d&iacute;a, mes y a&ntilde;o de la imagen adem&aacute;s del &aacute;rea de cada pol&iacute;gono en km<sup>2</sup>.&nbsp;</p>

<p>    <img width="164" alt="Imagen2" src="https://user-images.githubusercontent.com/101720220/204847431-b0cdcab8-63c9-4fb5-8620-ab93848dff49.png"  height="400">

</p>



<p>Figura 2: Pesta&ntilde;a mostrando las variables que debe seleccionar el usuario para realizar el mapeo y an&aacute;lisis de variaciones hist&oacute;ricas de lagos glaciares. N&oacute;tese que la &uacute;ltima opci&oacute;n (Descargar resultado Landsat) s&oacute;lo se activa y aparece cuando se ha ejecutado la herramienta. El nombre de ese hiperv&iacute;nculo cambia dependiendo de la colecci&oacute;n de im&aacute;genes seleccionada.</p>
<p>En la parte central de la interfaz se encuentra desplegado el mapa base. Se puede seleccionar el mapa base de Google o el mapa base satelital de Google. Estas opciones se encuentran ubicadas en la parte superior derecha del mapa (Figura 3). En esta pantalla el usuario debe delimitar el pol&iacute;gono de &aacute;rea de estudio -lago glaciar- que quiera analizar. Este pol&iacute;gono se dibuja con las herramientas de geometr&iacute;a ubicadas en la parte superior izquierda. El &aacute;rea seleccionada puede ser un rect&aacute;ngulo o pol&iacute;gono irregular. En esta pantalla se superpone autom&aacute;ticamente la imagen m&aacute;s reciente de la colecci&oacute;n analizada.</p>
<p>Figura 3:&nbsp; Mapa base e interfaz para delimitar lagos glaciares para el an&aacute;lisis. Se despliega la imagen m&aacute;s reciente de la colecci&oacute;n escogida (Landsat, Sentinel 1 o Sentinel 2).</p>
<p>Por &uacute;ltimo, en la parte en la parte derecha de la interfaz, se encuentran los resultados del an&aacute;lisis. En primer lugar, se visualizar&aacute; un <em>GIF</em> de las im&aacute;genes ocupadas por la clasificaci&oacute;n, con la opci&oacute;n de poder descargar a un disco local el archivo GIF de la animaci&oacute;n. Luego se mostrar&aacute;n los gr&aacute;ficos de c&aacute;lculo de &aacute;rea a trav&eacute;s de tiempo del lago glaciar seleccionado y la tasa de cambio de &aacute;rea (km<sup>2</sup>) entre im&aacute;genes sucesivas (figura 4)</p>
<p>&nbsp;Figura 4: Ventana&nbsp; de&nbsp; resultados mostrando en la parte superior animaci&oacute;n con las im&aacute;genes seleccionadas y en la parte inferior los gr&aacute;ficos de variaci&oacute;n hist&oacute;rica y tasa de cambio de la superficie de los lagos.</p>
<p>Los gr&aacute;ficos son interactivos y permiten inspeccionar la fecha y &aacute;rea estimada en cada imagen (e.i. en cada punto del gr&aacute;fico). Los gr&aacute;ficos tienen una pesta&ntilde;a en la parte superior derecha. Seleccionando esa pesta&ntilde;a se despliega una nueva ventana con el gr&aacute;fico seleccionado (Figura 5). En esta ventana se da la opci&oacute;n de descargar los datos del gr&aacute;fico en formato csv, o decargar el gr&aacute;fico mismo en formatos SVG y PNG.</p>
<p></p>
<p>Figura 5: Gr&aacute;fico de cambio de superficie de lago glaciar seleccionado. En la parte superior derecha se muestra las opciones de descarga de datos.</p>
