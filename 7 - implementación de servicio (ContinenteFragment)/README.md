# Haciendo funcionar el fragment de Continentes

Implementando el servicio de RestCountries para obtener infromación de paises por continente

## Preparando el Adaptador para  el RecyclerView

### Video
> [S7 - Creando clases PaisViewHolder y PaisAdapter](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/Eemsh5QBut1Ohl6f4BT5yBgB0RftgKhC2kpaTe6i3nL_Tg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=GpQTuy)
[![Creando clases PaisViewHolder y PaisAdapter](./thumbnail6.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/Eemsh5QBut1Ohl6f4BT5yBgB0RftgKhC2kpaTe6i3nL_Tg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=GpQTuy "Creando clases PaisViewHolder y PaisAdapter")

## Creando los objetos necesarios para trabajar

### Video
> [S7 - Definición de objetos e inicialización](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EaSj84oxXfRDpLj91kTUB7sBpq2IsQw4yZPaWqWuZhXa1w?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=ZbMKnf)
[![Definición de objetos e inicialización](./thumbnail1.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EaSj84oxXfRDpLj91kTUB7sBpq2IsQw4yZPaWqWuZhXa1w?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=ZbMKnf "Definición de objetos e inicialización")

## Solicitando la información a la Api

### Video
> [S7 - Método para traer información de la API](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/ER04rsdweUdAvCY8ZXgqc1UBafexviRt2npoVYe860ZcVA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=BExZ6N)
[![Método para traer información de la API](./thumbnail2.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/ER04rsdweUdAvCY8ZXgqc1UBafexviRt2npoVYe860ZcVA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=BExZ6N "Método para traer información de la API")

## Mandando la información al RecyclerView

Para hacer esto es neceario un permiso que se tiene que declarar en el archivo "AndroidManifest.xml", el permiso es el siguiente
```xml
    <uses-permission android:name="android.permission.INTERNET" />
```

### Video
> [S7 - Creando el adaptador del RecyclerView y limpiando la basura](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EZ_FSyIQbFRHrka2sWaT1C4B0aIh69okLRoucXi5PSkkyA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=vBAG5q)
[![Creando el adaptador del RecyclerView](./thumbnail3.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EZ_FSyIQbFRHrka2sWaT1C4B0aIh69okLRoucXi5PSkkyA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=vBAG5q "Creando el adaptador del RecyclerView")


## Añadiendo animación al country_recycler_item_layout
Código de la animación:
```xml
    <translate
        android:fromYDelta="-50%"
        android:toYDelta="0"
        android:duration="500"
        />

    <alpha
        android:fromAlpha="0"
        android:toAlpha="1"
        android:duration="500"
        />

    <scale
        android:fromXScale="125%"
        android:toXScale="100%"
        android:fromYScale="125%"
        android:toYScale="100%"
        android:pivotX="50%"
        android:pivotY="50%"
        android:duration="500"
        />
```

### Video
> [S7 - Animando la tarjeta de País](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/ETt06z1vIsxFsiTCtjxYAZkBlVFIoBS9xgStfx6M2NbHcA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=Vgy0m9)
[![Animando la tarjeta de País](./thumbnail5.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/ETt06z1vIsxFsiTCtjxYAZkBlVFIoBS9xgStfx6M2NbHcA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=Vgy0m9 "Animando la tarjeta de País")

## Haciendo funcionar el floating action button

### Video
> [S7 - Animando la tarjeta de País](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/ETt06z1vIsxFsiTCtjxYAZkBlVFIoBS9xgStfx6M2NbHcA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=Vgy0m9)
[![Animando la tarjeta de País](./thumbnail7.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/ETt06z1vIsxFsiTCtjxYAZkBlVFIoBS9xgStfx6M2NbHcA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=Vgy0m9 "Animando la tarjeta de País")

