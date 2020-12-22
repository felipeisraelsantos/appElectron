### App Electron para Desktop

É necessário ter o node instalado para verificar use o comando

```
$ node -v
```

caso não exista instalação acesse : https://nodejs.org/en/download/



## Inicializando projeto electron

Projeto criado com yarn ( mais o mesmo pode ser feito com npm )

```
$ yarn init -y
```

## Instalando o Electron

```
$ yarn add electron
```

## Instalando dependência " electron-builder"

```
$ yarn add electron-builder --save-dev
```

caso não seja riado o parametro devDependencies você pode criar  com os parâmetros

```
 "devDependencies": {
  	"electron-builder": "^22.9.1",
  	"electron": "^11.1.1"
  }
```



## Alterando o "package.json"

```
 "scripts": {
   "start": "electron .",
   "pack": "electron-builder --dir",
   "dist": "electron-builder",
   "dist:linux": "electron-builder --linux"
  }
```



## Gerando executal para linux

```
"build":{
   "linux": {
   "maintainer":"< autor >",
   "executableName":"< nome do app >",
   "category": "Utility",
   "target": [
      "deb"
      ]
   }
 }
```



execute o comando 

```
$ yarn dist:linux
```

