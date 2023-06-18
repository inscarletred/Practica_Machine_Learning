# Practica_Machine_Learning

Antes de empezar, te aviso que hay varios fallos en el código. He intentado corregirlo varias veces y no he podido. Me hubiera gustado dedicarle más tiempo, pero no he podido. Para no dejarla a medias, he seguido con el proceso a pesar de los errores para que puedas valorar tanto el código como el conocimiento del proceso.

Como hemos visto en clase, he seguido el siguiente proceso:

prepocesar PRE-división
        1) Quitar las columnas de: ID, scraped ID, URL, Lastscraped
            He quitado estas columnas porque sabiendo que el problema se trata de encontrar las variables que más influyen en el precio, sabemos que dichas columnas solo van a dar problemas
         2) Me he quedado con las entradas de Madrid (para hacerlo más facil, según recomendación)
         3) Check for Nas and NaNs. Despues de hacer el split entre train y test, habrá que ver si reemplazamos los NaNs o los dropeamos

Hacer el split:
    1) He hecho el split 75/25 de los datos, pero aqui es donde tengo el error que no soy capaz de arreglar. Por algun motivo tengo el y_test vacio, lo cual me da errores a partir de este chunk.
         
He hecho un check de los missing values en y_train, pero me dice que no hay? Igual es que no sé bien interpretar su respuesta. Intento dropear filas con
en test
He hecho correlation matrix con train y antes de romper el codigo he conseguido ver que las que tenian mejor correlacion eran: Precio y Accomodates, Precio y numero habitaciones, y precio y cleaning fee. 
 Despues he normalizado los sets, tanto train como test
he aplicado grid search y lasso para sacar los parametros más optimos y he calculado el MSE para valorar mi modelo. Dado el error con el y_test, no me ha funcionado ninguno de los dos y con lo cual no he podido interpretar bien los datos ni evaluarlo.
