# Request Header Parser Microservice

This is the code for the [Request Header Parser Microservice project at freecodecamp.org](https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/request-header-parser-microservice).

## How To Run The Code
1. Copy the file `env.example` and rename to `.env`. Fill the `PORT=` in `.env` with the port that the microservice will listen to.
2. Open terminal, and navigate to the directory where this code is located, and run `npm install`.
3. After finished installing dependencies, run `npm start`.
4. To test the api, you can use browser or [Postman](https://www.postman.com/downloads/). To send `GET` request on the browser, if the api is listening on `http://localhost:8080`, type `http://localhost:8080/api/whoami` and the api will give the response in `JSON` format.
5. To stop the api, type `Ctrl+C` in the terminal.

## Microservice Description
This Header Parser Microservice will handle API Endpoint at `/api/whoami`, the microservice will parse the request headers and then responds with the ip address, language, and then the user agent info, for example:
```Javascript
{"ipaddress":"::ffff:127.0.0.1","language":"en-US,en;q=0.5","software":"Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0"}
```