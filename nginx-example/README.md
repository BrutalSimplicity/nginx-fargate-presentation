Nginx Example

Pull Nginx Docker Image

`docker pull nginx:alpine`

Run Nginx Alpine Docker Image (but login with shell)

`docker run --rm -p 3000:80 -it nginx:alpine /bin/sh`

Build Custom Nginx Docker Image

`docker build . -f Dockerfile -t nginx-example`

Run Nginx Docker Image

`docker run --rm -p 3000:80 -d --name nginx nginx-example`

Attach to Running Docker Image via shell

`docker exec -it nginx /bin/sh`