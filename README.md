# How to use env files in Vue 3
In a web app, you will most likely have to access a backend API server through a URL. In a development environment - when you are working locally, this URL can be something like: http://localhost:8080/api. In a production environment - when the project has been deployed, this URL can be something like: https://example.com/api. Environment variables allow you to change this URL automatically, according to the current state of the project.

With Vue.js, it is possible to use environment variables through files with the .env file extension. These files are responsible for storing information that is specific to the environment (“development”, “testing”, “production”, etc.).

In this article, you will learn how to work with distinct configurations between development and production mode for Vue.js projects using Vue CLI 3+ and 2.
## Project setup
```
npm install
```

### Compiles and hot-reloads for development
If you compile the application with development values:
```
npm run serve
```
This command will use the .env value and will display: http://localhost/api.

If you compile the application with development values:
```
npm run serve -- --mode=production
```
This command will use the .env.production value and will display: http://www.example.com/api.

By default, Vue CLI will support three modes: “development”, "test’, and “production”.
