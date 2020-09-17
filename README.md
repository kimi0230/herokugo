# herokugo
Demo heroku

## Install the Heroku CLI
Download and install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-command-line).

## heroku login
```
$ heroku login
```

### Log in to Container Registry
You must have Docker set up locally to continue. You should see output when you run this command.
```
$ docker ps
```
Now you can sign into Container Registry.

```
$ heroku container:login
```

### Push your Docker-based app
Build the Dockerfile in the current directory and push the Docker image.

```
$ heroku container:push web
```

### Deploy the changes
Release the newly pushed images to deploy your app.

```
$ heroku container:release web
```

## Reference
https://blog.wu-boy.com/2019/02/deploy-golang-app-to-heroku/