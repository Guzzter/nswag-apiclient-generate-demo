# Getting Started NSwag client generation

This project demonstrates how to generate a client library for a web API using NSwag.

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the client-app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

Runs the server-app web api in the development mode.\
Open [http://localhost:5000/swagger](http://localhost:5000/swagger) to view swagger documentation in the browser.

### `dotnet run --project src/server-app/APIClientGenerator http://localhost:5000/swagger/v1/swagger.json src/client-app/src/WeatherForecastClient.ts TypeScript`

When API is running, this command will generate a TypeScript client library for the API.
It will store it in src/client-app/src/WeatherForecastClient.ts so that it can be used as TypeScript client lib in React client-app


### `dotnet run --project src/server-app/APIClientGenerator http://localhost:5000/swagger/v1/swagger.json WeatherForecastClient.cs CSharp`

When API is running, this command will generate a C# client library for the API.
