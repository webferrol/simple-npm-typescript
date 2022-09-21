# Proyeto node y TypeScript

## Tabla de contenidos

- [Arranque del proyecto](#npm-init)
- [Instalación de TypeScript](#instalación-de-typescript)
- [Configuración mínima de tsconfig.json](#configuración-de-tsconfig)

## npm init

Para arrancar el proyecto con una configuración mínima utilizaremos el comando de abajo. El parámetro -y es para que no nos pregunte nada

```sh
npm init -y
```

## Instalación de TypeScript

Para la instalación de typescript utilizar el siguiente comando. El _flag_ -D o el _parámetro_ --save-dev nos sirve para instalarlo como *dependencia de desarrollo*.

```sh
npm i -D typescript
```

## Configuración de tsconfig

Crearemos un fichero _tsconfig.json_ y crearemos una propiedad denominada "compilerOptions". Indicaremos la salida de _transpilación_ de los ficheros con extensión __ts__. El comando genérico es *tsc*

```json
{
    "compilerOptions": {
        "outDir": "dist",
        "target": "ES5"
    }
}
```

En el fichero _package.json_ podemos realizar en su propieda _scripts_ un automatismo para esta _compilación_.
