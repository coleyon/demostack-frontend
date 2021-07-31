# demostack-frontend

A snippet for creating my frontend app, based on the following projects
https://github.com/tiangolo/full-stack-fastapi-postgresql


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
        "type": "chrome",
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