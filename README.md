# Todo List Application

I am using this repository as a resume / portfolio example piece to show potential employers that I have a well rounded development skill set.

I chose to do a sample TODO list application from scratch, because it is sort of the "hello world" of a full fledge app. It requires all of the various components of an actual application.

The tools that I am using to write this app:

* Twitter Bootstrap
    * I use a custom theme from Bootswatch

* RactiveJS
    * Front end JS
    * 2 way data-binding


I also containerized the app to show that I know the basics of building, running and deploying web applications in Docker.

I used the base Apache container from https://hub.docker.com/r/appcontainers/apache/ and then cloned my git project into the container. I updated the apache conf file to work with my todo app and committed the changes. Then I pushed the image to the docker hub.

View the Container on the docker hub here: https://hub.docker.com/r/dsikes/todo/

If you run docker and would like to see the container run, simply do this:

    docker run -it -d --name todo -p 80:80 dsikes/todo

Depending on your setup, you should be able to navigate to localhost
(127.0.0.1) and view the web app running.

NOTE: THIS IS A SAMPLE APP. USE AT YOUR OWN RISK. :)