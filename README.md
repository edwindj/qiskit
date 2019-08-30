# Docker-image for qiskit-tutorial

This repo contains a Dockerfile that builds docker image with the qiskit tutorial


## Usage


1) Download this repo:

```
git clone git@github.com:edwindj/qiskit 
```

2) Run the container (with docker-compose)

```
sudo docker-compose up -d 
```

or plain docker

```
sudo docker build -t qiskit .
sudo docker run --rm -d -v $PWD/qiskit-iqx-tutorials/qiskit:/home/jovyan/qiskit -p 8888:8888 qiskit
```
A jupyter notebook with qiskit-tutorial installed will be running on http://localhost:8888.

3) First time login you will need a token. This can be found in the logs:

```
sudo docker-compose logs
# or
sudo docker logs <container_name>
```


Enjoy!


