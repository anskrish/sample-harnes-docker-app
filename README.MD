**This will help us to build the custom image for demo

* Update the content in site.html file

* Create a docker image

```
 docker build -t nginx-custorm:v2 .
```

* Push the image to repo

```
docker login
docker tag nginx-custorm:v2 <repo>
docker push <repo>
```

* Build the app

```
docker run -d -p 8080:80 --name web nginx-custorm:v2 

```

* Access the application

http://localhost:8080

