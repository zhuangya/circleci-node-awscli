[![Docker Automated build](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg?style=flat-square)](https://hub.docker.com/r/lfglore/circleci-node-awscli/)
[![Twitter URL](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://github.com/lfg-gaming/circleci-node-awscli)
# LFG-Lore's CircleCI docker image

### Intro
This image is based on [CircleCI's nodejs image](https://hub.docker.com/r/circleci/node/). Packages include
- Node: 9.0.0
- Python: 2.7.9
- AWS CLI: 1.11.181

### Build image
```
git clone https://github.com/lfg-gaming/circleci-node-awscli
cd circleci-node-awscli
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