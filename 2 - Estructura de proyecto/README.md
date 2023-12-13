# Definición de estructura de proyecto

En esta sección hablaremos de la estructura de proyecto a seguir y la cración de recursos a utilizar

## Videos
> [S2 - Creación de proyecto](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EfxwQtOSzFpCmRq1O5vdzHwBydCLdA9ePzMAdMJCUQX7OA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=jUgqUj)
[![Creación de proyecto](./thumbnail1.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EfxwQtOSzFpCmRq1O5vdzHwBydCLdA9ePzMAdMJCUQX7OA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=jUgqUj "Creación de proycto")

> [S2 - Creación de recursos, activities y fragments](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EW_XErOG5RBEop_YI_q6iD4BBw2nRNTe_NpGevF4H4XvGA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=DgB6Zk)
[![Creación de proyecto](./thumbnail2.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EW_XErOG5RBEop_YI_q6iD4BBw2nRNTe_NpGevF4H4XvGA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=DgB6Zk "Creación de proycto")


## Dependencias necesarias para trabajar

### Librearía para el consumo de servicios web (APIs) [Retrofit](https://square.github.io/retrofit/)


```c
    // Para Retrofit
    implementation("com.squareup.retrofit2:retrofit:2.9.0")
    implementation("com.squareup.retrofit2:adapter-rxjava2:2.9.0")
    implementation("com.squareup.retrofit2:converter-gson:2.9.0")
```

### Librería pára optimización de hilos [RxJava](https://github.com/ReactiveX/RxJava)

```c
    // Para RXJava
    implementation("io.reactivex.rxjava2:rxandroid:2.0.1")
    implementation("io.reactivex.rxjava2:rxjava:2.1.7")
```

### Librería [Glide](https://github.com/bumptech/glide) para carga de imágenes

```c
    // Para manejo de imágenes contenidas en servidor
    implementation("com.github.bumptech.glide:glide:4.16.0")
```

## Assets del proyecto

* Utilizados para este proyecto [aquí](./assets/)
* Si quieres buscar y utilizar tus propios recursos utiliza la web de [SVG Repo](https://www.svgrepo.com/)