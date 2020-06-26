# Curso de Gestión de Dependencias y Paquetes con NPM

## Crear credenciales en npm

- Email:

```
npm set init.author.email "value"
```

- Nombre:

```
npm set init.author.name "value"
```

- License:

```
npm set init.author.license "value"
```

## Instalación de dependencias

```
npm install/i nombrePaquete -flats
```

#### Flats

- --save/-S: Dependencia del proyecto.
- --save-dev/-D: Dependencia de desarrolo.
- --force/-f: Forzar la instalacion del paquete.
- -g: Dependencia global.
- -O: Dependencia opcional.
- --dd: Ver el funcionamiento de NPM.
- --dry-run: Simula la instalacion de la dependencia y muestra el output.

### Seleccionar una version especifica de uns dependencia

```
npm i nombre@version
```

## Actualizar paquetes

Ver que paquetes estan desactualizados.

```
npm outdate
```

Actualizar todos los paquetes.

```
npm update
```

Instalar la ultima version

```
npm i nombre@latest
```

## Eliminar paquetes

```
npm uninstall name
```

Desintalar un paquete sin eliminarlo del package.json

```
npm uninstall name --no-save
```

## Listar paquetes instalados de forma global

```
npm list -g --depth 0
```

#### Flats

- --depth:Profundidad en la cual va a buscar.0=todos
- -g: Paquetes globales.

## Package lock y el uso los símbolos ^ y ~

### Versionado

#### 1.0.0

- El primer valor represneta un cambio mayor.
- El segundo valor represneta un cambio menor.
- El tercero son parches o bun fixes

~:Indicamos que solo actualizaremos los parches y los bug fixes.
Caret(^): Indicamos que solo podamos actulizar los cambios menores y los parches o bug fixes.
