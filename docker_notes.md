# Again saving all the magic docker incantations

docker build -t phoenix_test_app -f Dockerfile_Phoenix_Test .

# Run a container inside bash

docker run --rm -it phoenix_test_app /bin/bash

# List built / downloaded images

# docker image list