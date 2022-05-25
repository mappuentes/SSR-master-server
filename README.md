# Ejemplo servidor para SSR
Bienvenidos a al servidor cloud para recibir dats

En /logs encontramos todos los archivos de log ordenados por fecha de creación

En el csv aparecerá cada entrada insertada en una línea, con su identificador, tiempo de inserción (en formato timestamp) y valores medidos.

Para insertar un conjunto de datos debemos realizar una petición HTTP GET hacia el punto /record, con los siguientes parámetros:

- id identificador del experimento que se ha realizado
- data valores medidos

Un ejemplo de inserción es la siguiente 
```
/record?id=nodo1&data=100
```
