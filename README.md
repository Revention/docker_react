## Frontend

#### <bold><font color="red">Important this project is still under development and my work differently than expected!!</font></bold>

### About

Frontend is an application made with react and nodejs. It is a simple webservice which you can run local, in the cloud or on server with a internet connection.

The purpose is to enable test-driven development and testing within a local environment running on docker. There is  a production node which can also be run on docker for selfhosting or on a internet-faced server or on a cloud service of your choice. Together you should have a complete CI/CD environment when deploying all the docker containers.

The docker images are build based on the sourcecode available on github : [github frontend](https://github.com/Revention/docker_react)

The docker images are available on dockerhub : [dockerhub frontend](https://hub.docker.com/repository/docker/revention/frontend/general)

### Runnng the container

#### Production
This docker image is optimized for running in a production environment and can be pulled from dockerhub by evoking the pull and/or run command. It is assumed you have docker installed on your system.

```docker pull revention/frontend:latest```


```docker run -p 8080:80 revention/frontend:latest```

```url: localhost:8080```

#### Test (version 0.3+)

The sourcecode is available on 
[github](https://github.com/Revention/docker_react.git)

<bold>Note: This version can differ from production!</bold>

1) Clone the git repository
```git clone https://github.com/Revention/docker_react.git```
[github](https://github.com/Revention/docker_react.git)
3) Build and start the development test environment
```docker compose up```
4) In another terminal window
```docker exec -it frontend-test-1 sh```
5) Open a browser
[Test-environment](http://localhost:3000)

#### Alternative

```docker run -it revention/frontend:test-latest npm run test```


#### Version 2.0 or prior
```bash
docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app --rm --name dev --hostname develop  revention/frontend
```

#### Docker-compose
```bash
docker compose up
```


### URL
http://localhost:3000/


# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
