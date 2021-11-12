# demostack-frontend

A snippet for creating my frontend app, based on the following projects
This code is disassembled codes for understanding and applying the original design. Only use for learning.

https://github.com/tiangolo/full-stack-fastapi-postgresql

**Modifications**:

In shortenaly, this code is degraded version of the original. 

* Split the frontend and the backend into two different projects
* Removed Traefik routing and simplified Dockerfile

backend project is here: https://github.com/coleyon/demostack

# howto up-down

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Run your unit tests
```
npm run test:unit
```

# local debug settings

`.vscode/launch.json`

```json
{
    "version": "0.2.0",
    "configurations": [
      {
        "type": "pwa-chrome",
        "request": "launch",
        "name": "chrome",
        "url": "http://localhost:8080",
        "webRoot": "${workspaceFolder}/src",
        "preLaunchTask": "serve",
        "breakOnLoad": true,
        "sourceMapPathOverrides": {
        "webpack:///./src/*": "${webRoot}/*"
      }
    }
  ]
}
```

# node

```bash
$ nvm install 10.24.1
$ nvm use 10.24.1
$ node --version
v10.24.1
$ npm install
```
