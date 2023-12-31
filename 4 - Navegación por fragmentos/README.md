# Navegación a través del elemento BottomNavigationview

En esta sección habilitaremos la navegación a través del elemento mencionado

## Videos
> [S4 - Creación del menu para navegación](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/ERVO90u_GYpNi6r10heexZ0B8QEmy03te27iGEH6tZD0vA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=yftwi2)
[![Creación de proyecto](./thumbnail1.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/ERVO90u_GYpNi6r10heexZ0B8QEmy03te27iGEH6tZD0vA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=yftwi2 "Creación de proycto")

> [S4 - Creando componente de mavegación](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EXKdlA-K8ApCiICw3pXkYnwBKIR5NAPL23U4gIEv6r3Vig?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=jxNovh)
[![Creación de proyecto](./thumbnail2.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EXKdlA-K8ApCiICw3pXkYnwBKIR5NAPL23U4gIEv6r3Vig?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=jxNovh "Creación de proycto")

> [S4 - Haciendo funcionar la navegación](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EUnXRhIq-tNFrnBXk_unvpwBX43F-2rgSkOwt-FBos8LjA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=sqZblF)
[![Creación de proyecto](./thumbnail3.png)](https://itcgedu-my.sharepoint.com/:v:/g/personal/m21290940_cdguzman_tecnm_mx/EUnXRhIq-tNFrnBXk_unvpwBX43F-2rgSkOwt-FBos8LjA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=sqZblF "Haciendo funcionar la navegación")

## Menu items
Estos son los menu items que tienen que crear para la navegación
```xml
     <item
        android:id="@+id/mainNavMiContinente"
        android:icon="@drawable/ic_world_25"
        android:title="@string/mainNavMiContinente"
        android:enabled="true"
        />

    <item
        android:id="@+id/mainNavMiBuscar"
        android:icon="@drawable/ic_map_search_25"
        android:title="@string/mainNavMiBuscar"
        android:enabled="true"
        />

    <item
        android:id="@+id/mainNavMiPerfil"
        android:icon="@drawable/ic_profile_25"
        android:title="@string/mainNavMiPerfil"
        android:enabled="true"
        />
```

## Definición de elementos activos para la navegación
Estos son los elementos que deberán tener en el atchivo de "main_navigation_component.xml"
```xml
    <fragment
        android:id="@+id/mainNavMiContinente"
        android:name="com.m21290940.mycountryapp.paises.fragments.PorContinenteFragment"
        android:label="Paises por continente"
        tools:layout="@layout/fragment_por_continente" />

    <fragment
        android:id="@+id/mainNavMiBuscar"
        android:name="com.m21290940.mycountryapp.paises.fragments.BuscarPaisesFragment"
        android:label="Buscar País Por Nombre"
        tools:layout="@layout/fragment_buscar_paises" />

    <fragment
        android:id="@+id/mainNavMiPerfil"
        android:name="com.m21290940.mycountryapp.perfil.fragments.PerfilFragment"
        android:label="Desarrollador"
        tools:layout="@layout/fragment_perfil" />
```