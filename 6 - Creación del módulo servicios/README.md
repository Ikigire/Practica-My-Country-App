# Creando la representación de la API para la extracción de datos de un servidor

## Servicio a consumir

La Api a consumir será la api de [RestCountries](https://restcountries.com/) la cual es capaz de abastecer de información acerca de paises

### Video
> [S6 - Presentación de la API a consumir](https://1drv.ms/u/s!AvB-2ztiY9QqgpUeVTKueS7SK45iDQ?e=V5SOgJ)
[![Creación de proyecto](./thumbnail1.png)](https://1drv.ms/u/s!AvB-2ztiY9QqgpUeVTKueS7SK45iDQ?e=V5SOgJ "Presentación de la API a consumir")

## La librería [Retrofit](https://square.github.io/retrofit/)

Siempre que vayan a implementar una librería deben de asegurarse de leer la documentación oficial o por lo menos visitar o ver algún sitio o video acerca de la librería

### Video
> [S6 - Librería Retrofit](https://1drv.ms/u/s!AvB-2ztiY9QqgpUfH7_gMVgB8-XJpg?e=DOWU9U)
[![Creación de proyecto](./thumbnail3.png)](https://1drv.ms/u/s!AvB-2ztiY9QqgpUfH7_gMVgB8-XJpg?e=DOWU9U "Librería Retrofit")

## Definición de Modelos

Para asegurar que ustedes tengan accesso a la de finición de modelos deberán de copiar el contenido del archivo ["countries.json"](./countries.json) que está en esta misma sección.

Además deberán de acceder a la páginade [Quicktype](https://quicktype.io/) para obtener el código de manera fácil

### Video
> [S6 - Creación de modelos](https://1drv.ms/u/s!AvB-2ztiY9QqgpUgrCO2Yea8yJHh3g?e=d894nh)
[![Creación de proyecto](./thumbnail2.png)](https://1drv.ms/u/s!AvB-2ztiY9QqgpUgrCO2Yea8yJHh3g?e=d894nh "Creación de modelos")


## Generando la interfaz para consumo de la API

Para poder invocar los métodos disponibles dentro de la API hay que generar una interfaz de que permita conectarse bajo las reglas de la API

Valor para los filtros:
```java
  "?fields=name,cca3,flag,flags,capital,population"
```

### Video
> [S6 - Definiendo interfaz API](https://1drv.ms/u/s!AvB-2ztiY9QqgpUhG19bITVhJd6xWg?e=S6s0wg)
[![Creación de proyecto](./thumbnail4.png)](https://1drv.ms/u/s!AvB-2ztiY9QqgpUhG19bITVhJd6xWg?e=S6s0wg "Definiendo interfaz API")


## Creación del Cliente

La forma de realizar la conexión con la API es a través de un cliente, dicho cliente es que implementará la interfaz creada para poder traer datos de la API

Valor del BASE_URL:
```java
    "https://restcountries.com/v3.1/"
```

### Video
> [S6 - Creando el cliente de la API](https://1drv.ms/u/s!AvB-2ztiY9QqgpUjqf9PK3Tme26GRw?e=b0VR3b)
[![Creación de proyecto](./thumbnail5.png)](https://1drv.ms/u/s!AvB-2ztiY9QqgpUjqf9PK3Tme26GRw?e=b0VR3b "Creando el cliente de la API")


## Complemento: Preparando la utilización de filtro "fields"

### Video
> [S6 - Preparando la variable de los filtros](https://1drv.ms/u/s!AvB-2ztiY9QqgpUiZwJoiOW0ZnjJAg?e=ETqOYg)
[![Creación de proyecto](./thumbnail5.png)](https://1drv.ms/u/s!AvB-2ztiY9QqgpUiZwJoiOW0ZnjJAg?e=ETqOYg "Preparando la variable de los filtros")
