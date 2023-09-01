# docker-practice

This is a simple docker practice project. It contains a simple web application written in html. The web application is hosted using nginx web server. The docker image is built using a Dockerfile.

## Clone repository
```bash
git clone https://github.com/LakshanRukantha/docker-practice.git
```

## Change directory
```bash
cd docker-practice
```

## Build image
```bash
docker build -t docker-practice .
```

## Run container
```bash
docker run -d -p 8080:80 docker-practice
```

## Test
```bash
curl http://localhost:8080
```

## Push image to docker hub
```bash
docker login
docker tag docker-practice lakshanrukantha/first-repo
docker push lakshanrukantha/first-repo
```

## Pull image from docker hub
```bash
docker pull lakshanrukantha/first-repo
```