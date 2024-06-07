
## Módulo 1 - LAYOUT - Laboratorio 1 (Ejercicio Nº1 - Nº2)

El proyecto se ha generado con el builder Vite.
Para arrancar la aplicación es necesario ejecutar los siguientes comandos en la carpeta src:
```
npm install
npm run dev
```

`Ejercicio Nº1`
El código de Scss se inyecta directamente en el HTML gracias a Vite, por lo que tenemos la carpeta mas limpia de ficheros, libre de compilaciones.
Para el desarrollo del código he creado los siguientes archivos:
- _mixins.scss (donde se almacenan todos los mixins de forma parcial)
- _variables-scss (donde se almacenan las variables de forma parcial)
- style.scss (el archivo principal de los estilos)

En términos generales, he creado una composición de mixins con una lógica para poder insertar por parámetro los siguientes datos :
>>**color base** / **nº de hijos** / **intensidad color paleta**

Todo esto se debe modificar en el archivo style.scss, en la clase de cada contenedor padre y aplicándolo en la declaración del @include como en el ejemplo siguiente:
```
 @include color-palette($color-red-base, 4,20);
```

`Ejercicio Nº2`