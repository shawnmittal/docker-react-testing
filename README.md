# React with Docker and AWS

[![Build Status](https://travis-ci.com/shawnmittal/docker-react-testing.svg?branch=main)](https://travis-ci.com/shawnmittal/docker-react-testing)

Testing out React usage with Docker for dev and deployment with AWS Elastic Beanstalk.

## Using Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## React Leaflet App
Application is a leaflet based app based on [https://github.com/scottpdawson/react-leaflet-maps](https://github.com/scottpdawson/react-leaflet-maps).

### Development Notes

## Build Docker Dev
`./scripts/docker-dev-build.sh` builds the docker image with the npm dependencies. Allows for live edits of the code to be reflected at [http://localhost:3000](http://localhost:3000) by volume mounting `$(pwd):/app`.

## Run Tests
`./scripts/docker-dev-test.sh` runs npm test on `shawnmittal/docker-react-testing:dev` after build.

## Run Dev Container
`./scripts/docker-dev-run.sh` runs the docker development container and starts the npm development server at [http://localhost:3000](http://localhost:3000).
