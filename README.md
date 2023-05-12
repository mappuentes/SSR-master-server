# Data-Logger
Bienvenidos a Data-Logger

En /logs encontramos todos los archivos de log ordenados por fecha de creación

En el csv aparecerá cada entrada insertada en una línea, con su identificador, tiempo de inserción (en formato timestamp), frecuencia y valores medidos.

Para insertar un conjunto de datos debemos realizar una petición HTTP GET hacia el punto /record, con los siguientes parámetros:

- id identificador del experimento que se ha realizado
- frec frecuencia de muestreo de las medidas
- data valores medidos separados por comas

Un ejemplo de inserción es la siguiente 
```
/record?id=experimentoPrueba1&data=0.1,0.2,0.1,0.3,0.4&frec=100
```
