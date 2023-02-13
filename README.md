![image](https://user-images.githubusercontent.com/117199136/218277519-421a9ba6-4324-4aac-bfb9-c388f61ad53d.png)

En este proyecto he querido ver o al menos intentar buscar las posibles causas de por qué un país desarrollado como es EEUU tiene tan alto indice de de delicuencia o criminiladid. Para ello me he basado en un dataset con una muestra aleatoria de ciertos delitos que se cometen en los EEUU y por estado. 

por qué he escogido por cada estado?

Me pareciá curioso comprobar si ciertos aspectos o variables podrían afectar a dicho estudio. Por tanto una vez tengo el dataset he iniciado mis indagaciones.

Partiendo del dataset original lo primero que se me ocurrió fue añadir una columna de ratio de crimenes por estado. Además he obtenido el link de una imagen en la que sale el mapa de los estados unidos con sus estados coloreados por tasa de crimenes.

![image](https://user-images.githubusercontent.com/117199136/218307965-d47ce7f2-7a5d-4e83-8085-943aacbfd4fa.png)


Para llevar a cabo lo arriba mencionado he usado el método de scraping por selenium bien para la fotografia bien para la obtención de la columna requerida.Una vez he obtenido los datos al no estar correctamente los he limpiado mediante la formula 'replace' quitando todo tipo de espacios y números que no necesitaba.

Teniendo en cuenta ya esta variable he procedido a añadir otra más. Esta vez la de renta familiar por estado. Esta variable la he obtenido por el método de scraping de beautifulsoup.

Finalmente me he descargado otro CSV con varias columnas.Aquí he tenido mis dudas si dejar dos dataframes que los podría unir en SQL o si por el contrario dejaba solo un dataframe pero añadiendole las columnas del segundo dataframe. Al final he optado por la última ya que uno de mis fines era aprender ha hacer correlaciones por lo que he juntado las columna que queria en este caso la tasa de alcoholemia al dataframe original.Quedando una tabla tal que así:

![image](https://user-images.githubusercontent.com/117199136/218306324-9e211725-a604-472e-b279-9a02540ab188.png)

Teniendo ya la tabla empiezo ha hacer mis cabalas. Como he indicado más arriba había dudado de si hacer las relaciones en SQL o mediante correlaciones y bucles en Pandas y al final decicí por esto último ya que el fin de semana pasado en el proyecto de SQL profundizamos bastante el tema.

Como podeís observar en la primera de las correlaciones la conclusion es que ni los asesinatos ni la renta de las familias influyen en el consumo de alcohol al tener una correcilacion cercana a 0. 
En cambio los asesinatos tienen una correlación más baja con la renta por lo que a más renta menos asesinatos(también tiene lógica).

![image](https://user-images.githubusercontent.com/117199136/218307345-db39b386-6679-4066-977c-2d6db360c1e2.png)

Añado otra de mis conclusiones con otra correlación:

![image](https://user-images.githubusercontent.com/117199136/218307692-4c3b5b25-9cdd-4609-9253-331738db67b9.png)

Conclusion la tasa de crimen no tiene tanta correlacion con la tasa de alcohol como se pensaba.


Y para finalizar hago un bucle que me relaciones ciertas variables:

![image](https://user-images.githubusercontent.com/117199136/218307775-c9d5cfe8-cfbf-43da-bb95-ce178a7bceca.png)

Y en SQL quedaría tañ que así:

![image](https://user-images.githubusercontent.com/117199136/218469182-0472f5db-ffef-44cd-a21f-3c18c5ea5d9f.png)





