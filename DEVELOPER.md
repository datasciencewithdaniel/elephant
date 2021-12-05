# Developer Guide

To access the source code, clone the repository using Git as follows:

```
git clone https://github.com/datasciencewithdaniel/elephant.git
```

OLD:

```
docker build -t elephant .
docker-compose run --rm --service-ports elephant /bin/bash
```

NEW:

```
docker build -f Dockerfile -t elephant-app .
docker run --rm -p 3000:3000 elephant-app
```

NEW2:

```
docker build -f Dockerfile.api -t elephant-api .
docker build -f Dockerfile.client -t elephant-client .
docker-compose up --build
```