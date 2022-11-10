- ETL:

Utilice python (Numpy, Pandas) para la extraccipon y transformación de los datos. Para su carga primero arme una base de datos en MySQL y luego realice una conexión por medio de SQLAlchemy de Python con la DB para cargar los registros.


- EDA:

    Diccionario de Variables:

    index: índece del dataset
    date : fecha del accidente
    time : hora declarada en la que se produjo el accidente
    location : ubicación del accidente
    operator : responsable del vuelo
    flight_no : número de vuelo
    route : objetivo del vuelo, describe una actividad o un trayecto(origen,destino)
    ac_type : tipo de aeronave
    registration : matrícula de la aeronave
    cn/In : Número de serie de la aeronave
    all_aboard : personas a bordo
    passenger_aboard: pasajeros a bordo
    total_deaths
    passenger_fatalities : cantidad de pasajeros fallecidos
    crew_fatalities : cantidad de tripulantes fallecidos
    ground : cantidad de víctimas terrestres
    Summary : descripción


    El dataset otorgado no presenta registros duplicados.
    Observar que no hay registros con valores nulos, donde faltan datos está indicado con el símbolo '?'.

    Los datos en general están completos en su totalidad, concentrandose la mayor cantidad de datos faltantes en columnas de menor relevancia.

    Trabajé sobre las columnas 'date' y 'time' ya que había que normalizarlas, presentaban un tipo de dato incorrecto y particularmente 'time' contienía una gran cantidad de registros con caracteres especiales.

    El problema de valores faltantes lo resolví para variables cualitativas indicando 'sin dato' y en las cuantitativas elimine los registros debido a que representaban una proporcion baje en comparacion con el total de muestras.

    Los outliers detectados corresponden a accidentes reales, uno de estos casos es el accidente entre pan american world airways y klm en Tenerife, Canary Islands que fue el accidente aéreo más grave de 1977 y el más catastrófico en una colisión aérea en tierra. Otros outliers hacen alusión a lo sucedido el 11 de septiembre de 2001 con el atentado a las Torres Gemelas.

    Para analizar los datos tome distintas estrategias, como:

        - Representar con una nube de palabras el contenido de la columna 'summary' en busca de información relevante.
        - Determinar localidades con más accidentes fatales
        - Hallar fechas con más accidentes fatales
        - Detectar que aerolínea presenta mayor cantidad de accidentes fatales
        - Buscar colisiones entre aviones.
 
    Por último con los conocimientos que obtuve sobre el dataset me decidí por 'Colisiones entre aviones' como base para realizar mi presentación.



