# This is test api for docker container and other research

## Create a .net api project

# 1) Create the project with controllers
dotnet new webapi --use-controllers -o MyApi

# 2) Open in VS Code
code -r MyApi

# 3) Run
dotnet run

# 4) Open in browser
http://localhost:5215/api/WeatherForecast

## Add .dockerignore for docker
.dockerignore

## Add dockerfile to create docker image
Dockerfile

# How to run in docker
1. docker build -t testapi . (used to build the image)
2. docker run -p 5215:80 testapi (used to run the image)
3. http://localhost:5215/api/WeatherForecast (used to open the api in browser which is running in docker)

## Add docker-compose.yml
docker-compose.yml

# How to run in docker
1. docker-compose up -d (used to run the image)
2. http://localhost:5215/api/WeatherForecast (used to open the api in browser which is running in docker)   
