![image](https://user-images.githubusercontent.com/117199136/218277519-421a9ba6-4324-4aac-bfb9-c388f61ad53d.png)

En este proyecto he querido ver o al menos intentar buscar las posibles causas de por qué un país desarrollado como es EEUU tiene tan alto indice de de delicuencia o criminiladid. Para ello me he basado en un dataset con una muestra aleatoria de ciertos delitos que se cometen en los EEUU y por estado. 

por qué he escogido por cada estado?

Me pareciá curioso comprobar si ciertos aspectos o variables podrían afectar a dicho estudio. Por tanto una vez tengo el dataset he iniciado mis indagaciones.

Partiendo del dataset original lo primero que se me ocurrió fue añadir una columna de ratio de crimenes por estado. Además he obtenido el link de una imagen en la que sale el mapa de los estados unidos con sus estados coloreados por tasa de crimenes.

Para llevar a cabo lo arriba mencionado he usado el método de scraping por selenium bien para la fotografia bien para la obtención de la columna requerida.Una vez he obtenido los datos al no estar correctamente los he limpiado mediante la formula 'replace' quitando todo tipo de espacios y números que no necesitaba.

Teniendo en cuenta ya esta variable he procedido a añadir otra más. Esta vez la de renta familiar por estado. Esta variable la he obtenido por el método de scraping de beautifulsoup.

Finalmente me he descargado otro CSV con varias columnas.Aquí he tenido mis dudas si dejar dos dataframes que los podría unir en SQL o si por el contrario dejaba solo un dataframe pero añadiendole las columnas del segundo dataframe. Al final he optado por la última ya que uno de mis fines era aprender ha hacer correlaciones por lo que he juntado las columna que queria en este caso la tasa de alcoholemia al dataframe original.Quedando una tabla tal que así:




