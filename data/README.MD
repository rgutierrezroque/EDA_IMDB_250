# Base de datos IMDB_Top_250_Movies.csv

Esta base de datos contiene la información básica de las 250 peliculas mejor puntuadas en el portal imdb.com

|Campo          |Tipo       |Descripción                            |Notas   |   |
|---------------|-----------|---------------------------------------|---|---|
|rank           |entero     |Posición de la película en el TOP250   |Valor 1 a 250   |   |
|name           |texto      |Nombre de la película                  |Nombre en idioma original   |   |
|year           |entero     |Año de estreno                         |   |   |
|rating         |decimal    |Calificación                           |Otorgado por usuarios   |   |
|genre          |texto      |Generos                                |Lista con los generos a los que pertenece   |   |
|certificate    |texto      |Clasificación                          |Clasificación asignado en el pais de origen   |   |
|run_time       |texto      |Duración                               |Medido en horas y minutos    |   |
|tagline        |texto      |Eslogan                                |En Ingles   |   |
|budget         |entero     |Presupuesto                            |En dolares   |   |
|box_office     |entero     |Ingresos en la apertura                |En dolares   |   |
|casts          |texto      |Elenco                                 |Lista de el elenco principal   |   |
|directors      |texto      |Directores                             |Lista de los directores   |   |
|writers        |texto      |Escritores                             |Lista de los escritores   |   |


La pregunta que quiere responder esta relacionada a la ganancia, pero dado que los valores proporcionados no estan actualizados a la inflación actual, utilizaremos un valor agregado calculando la proporción entre el box_office respecto al presupuesto en valores originales. Este campo lo llamaremos ganancia_proporcional.

$$ ganancia proporcional = {boxoffice \over budget} $$

## Notas
- El portal esta basado en los Estados Unidos y aunque se supone que tiene una base de usuarios global, no podemos omitir este hecho que puede crear una tendencia hacia las peliculas de ese pais.
- La industria cinematografica esta dominada por Estados Unidos y eso crea nuevamente una tendencia igual en ese sentido.
- La mayoria de la información original esta en ingles y los datos economicos en dolares Estadounidenses.








