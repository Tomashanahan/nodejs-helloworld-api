## Configuración del Pipeline de Jenkins

        1. Clonar/Forkear el repositorio
        2. Configurar Jenkins
            a. Crear la credencial para el repositorio
            b. Instalar el plugin de Nodejs
            c. Configurar en Tools el nuevo plugin de Nodejs seleccionando idealmente la versión 21.7.1
            d. Ir a la configuración de el pipeline y seleccionar la opción "GitHub hook trigger for GITScm polling?" para poder escuchar eventos de github
        3. Configurar ngrok
            a. correr el comando "HTTP http://<TU_IP>:<PUERTO_DE_TU_JENKINS>/"
            b. copiar la URL generada por ngrok para luego pegarla en el weebhook de github
        4. Configurar github
            a. Ir a la configuración > webhook del repositorio y seleccionar "Add webhook"
            b. Pegar la URL de gnrok.

### Ejecutar el Pipeline

Luego de todas las configuraciones previamente listadas, para poder testear que el pipeline esté funcionando de forma correcta, podemos hacer un pequeño cambio en el repo para luego hacer un push y así corroborar que el webhook se activa

# NodeJs, helloworld API for test propouses.

This is a simple API that returns a welcome message.

## Run your local environment

### Clone the repository

```bash
git clone https://github.com/edgaregonzalez/nodejs-helloworld-api.git
```

### Install dependencies

```bash
npm install
```

### Run the tests

```bash
npm test
```

### Start the server

```bash
npm start
```

### Make a request

```bash
curl http://localhost:3000
```
