# Qué es ESLint

EsLint es sencillamente una herramienta de linting para _JavaScript_ y _JSX_ cuya función es la de revisar nuestro código tratando de encontrar errores que podrían provocar problemas de compilación o bien futuros bugs en nuestro desarrollo. Cuando EsLint encuentra algún error, o bien lo repara de forma automática o bien nos advierte de ello a través de distintos mensajes, basándose para ello en un conjunto de reglas definidas previamente y que son altamente configurables.

Podemos encontrarnos con dos tipos de reglas. Unas encaminadas a garantizar la calidad de nuestro código, como por ejemplo la detección de variables declaradas o funciones que no se están usando en nuestro código, y otras encaminadas a garantizar que el formato de nuestro código mantiene cierta homogeneidad, como por ejemplo el uso de puntos y comas al final de nuestras instrucciones, espaciados, etc.

También podremos configurar nuestras propias reglas de linting o bien usar algunas de las extensiones de estilo que ya usan ciertas empresas como por ejemplo [Google](https://google.com) o [AirBnB](https://airbnb.com). Tal y como se analiza en este post, parece que las usadas por AirBnB son las más extendidas y son las que usaremos en el ejemplo de configuración que veremos continuación.

## Configuración de ESLint en nuestro proyecto

Para comenzar a usar EsLint en nuestro proyecto deberemos, en primer lugar, instalar las dependencias de desarrollo necesarias:

1. Instala EsLint & Prettier extensions para VSCode.

2. Instala los siguientes paquetes.

`npm i --save-dev eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-node eslint-config-node`

`npx install-peerdeps --dev eslint-config-airbnb`

3. Crear .prettierrc para cualquier regla de prettier (semicolons, quotes, etc).

4. Crea un fichero con eslint desde la terminal, puedes ejecutar el siguiente comando en tu terminal.

`eslint --init`

Esto generará un fichero .eslintrc

5. Haz pruebas con _ESLint_.
