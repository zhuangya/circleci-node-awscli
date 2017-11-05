# LFG-Lore's CircleCI docker image

### Intro
This image is based on [CircleCI's nodejs image](https://hub.docker.com/r/circleci/node/). Packages include
- Node: 9.0.0
- Python: 2.7.9
- AWS CLI: 1.11.181

### Build image
```
git clone https://github.com/lfg-gaming/circleci-docker.git
cd circleci-docker
docker build -t lfglore/circleci-node-awscli:latest .
```

### Push to Docker Hub
```
docker push lfglore/circleci-node-awscli:latest
```

### Pull from Docker Hub
```
docker pull docker pull lfglore/circleci-node-awscli:latest
```

### Run image
```
docker run -it lfglore/circleci-node-awscli bash
```

### Use as base image
```Dockerfile
FROM lfglore/circleci-node-awscli:latest
```