This application will be forked from https://github.com/LawrenceDavy13/weatherapp, as this project will be focused on the cloud/server side of devops not the developer side.

For this section we going to deploy a microservice application using continuous integration and continuous delivery. The application will be service that allows the user to enter a city name and get the current weather conditions of their city. The app gets its weather data from public API. Each service is run through a Docker container so that they can later be deployed on Kubernetes.

The app contains three microservices. The authentication service (written in Golang) and is responsible for creating user accounts, authenticating users and stores its data in the MYSQL database.

The UI service (written in JavaScript/NodeJS) is responsible for displaying the user interface and weather conditions. When the user creates an account or tries to log into the UI, the authentication service grants access to the user by returning an authentication cookie and gets stored in the browser by the UI service. When the user enters the city name in the text box, the UI service can message the weather service (written in Python).

The weather service contacts the public API and authenticates itself to the is public API using a API key. Once the weather service gets the requires data, it returns it back to the UI service to be displays to the user.
