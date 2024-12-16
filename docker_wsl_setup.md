# Docker via Windows Subsystem for Linux

Install docker for windows as normal: https://docs.docker.com/desktop/features/wsl/

Ensure during setup WSL is installed (done) and install if needed

Settings From the General tab, select Use WSL 2 based engine.

## Test it

To test docker instalation from WSL:

`docker run --rm -it python:latest python`

