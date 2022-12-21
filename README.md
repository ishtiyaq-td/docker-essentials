# Docker Essentials

## Important docker commands

```bash
doceker info
docker version
docker search
docker pull
docker run
docker ps
docker stop
docker restart
docker kill
docker exec
docker login
docker commit
docker push
docker network
docker history
docker rmi
docker ps -a
docker copy
docker logs  
docker volume
docker logout
docker exec
docker logs
docker rm
docker search
```

## Installation guide

### **Install git**

[https://git-scm.com/downloads](https://git-scm.com/downloads)

### **Install docker**

[https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/)

## Setup steps

1. Clone the project repository by running:

    ```bash
    git clone <REPO_URL>
    ```

2. Navigate to the nginx-website folder by running:

    ```bash
        cd docker-essentials-demo
    ```

3. Build the docker image by running:

    ```bash
        docker build . -t nginx-website:latest
    ```

    > Note: this assumes the Dockerfile is in the directory you are running this command

4. Run the newly built image to check out the website in a browser

    ```bash
        docker run -p 8088:80 docker-essentials-demo:latest
    ```

    This creates a new container from the image and binds port 80 of the container to port 8088 of the host machine

5. Visit `http://127.0.0.1:8088` or `http://localhost:8088` to view the website

    Click `ctrl+c` to stop the running container.

> Note: I did not make this website but I downloaded it from [https://github.com/learning-zone/website-templates](https://github.com/learning-zone/website-templates)