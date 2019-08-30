# Docker-image for qiskit-tutorial

This repo contains a Dockerfile that builds docker image with the qiskit tutorial


## Usage

Download this repo:

```
git clone git@github.com:edwindj/qiskit 
```

And go: (with docker-compose)

```
sudo docker-compose up -d 
```

or plain docker

```
docker build -t qiskit .
docker run --rm -d -v $PWD/qiskit-iqx-tutorials/qiskit:/home/jovyan/qiskit -p 888:8888 qiskit
```

And a jupyter notebook with qiskit-tutorial installed will be running on http://localhost:8888. Enjoy!

