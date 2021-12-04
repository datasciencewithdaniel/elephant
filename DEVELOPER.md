# Developer Guide

To access the source code, clone the repository using Git as follows:

```
git clone https://github.com/datasciencewithdaniel/elephant.git
```

Once you have installed Docker on your system, run the following command to build the image from the root directory of the repository:

```
docker build -t elephant .
```

Once the image has been built (remembering that future changes may require additonal builds), you can run the following command from the root directory of the repository to access a bash terminal for development:

```
docker-compose run --rm --service-ports elephant /bin/bash
```
