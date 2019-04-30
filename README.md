# forked sample-node-app

Forked habitat [project](https://github.com/habitat-sh/sample-node-app) .
Habitat is cool.



## prerequisite

 - docker
 - habitat cli

## how to build and run

Enter habitat studio-shell with
````
$ hab studio
````
When in hab-shell, use this obvious command to build project with all dependencies:
````
$ build
````
To later run the app in docker, use this command to create a docker image with the project:
````
$ hab pkg export docker ./results/<YOURE_ORIGIN>.hart
````
To find the docker image and its name, use:
````
$ docker images
````
To run the docker application:
````
docker run -it -p 8000:8000 <YOUR_ORIGIN>/sample-node-app
````
![habitat-sample-node-app](https://user-images.githubusercontent.com/274700/39158589-d1170792-4715-11e8-8e2a-1a2696944500.png)
