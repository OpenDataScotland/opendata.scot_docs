---
title: "How to: run frontend locally"
---

# How to: run frontend locally

To run the opendata.scot website locally

The easiest way to do this is with Docker. Download and install docker if not already installed https://docs.docker.com/get-docker/
There is no need to complete the tutorial.

In terminal
1. With Docker installed (check if installed with `docker --version`)
2. Navigate to JKAN repository
3. Run `docker compose up`
4. In your browser of choice, enter the server address `http://0.0.0.0:4000/` in the address bar
5. When you're done, hit `CTRL+C` to kill the docker process.


The first time `docker compose up` is run it will take a few minutes to setup the container. Subsequent loads will be quicker.
If the docker container needs to be rebuilt in case of cacheing issues, run `docker compose down` followed by `docker compose up` to start it again.