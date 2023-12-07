# Definición de estructura de proyecto

En esta sección hablaremos de la estructura de proyecto a seguir y la cración de recursos a utilizar

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
