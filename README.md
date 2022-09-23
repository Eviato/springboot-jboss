# Springboot out of the box on JBOSS App Service.

> This repository will contains a hello world application generated with SpringBoot Framework to be deployed on a Azure App Service.

## Architecture considerations

Create a app service with runtime Java11 and server set to JBOSS EAP 7

## Build the project

Build the project with `mvn clean package`

It will generate a `.war` file in the `target/` folder.

## Deploy the app

You can deploy the application using:

`az webapp deploy -g $RESOURCE_GROUP_NAME --name $APP_SERVICE_NAME --src-path target/demo-0.0.1-SNAPSHOT.war --type war`
