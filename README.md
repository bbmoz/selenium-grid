# Selenium Grid

> Spin up your own selenium grid on a docker container with minimal configuration.

## Tasks
1. `make start` or `make` to start the grid with a hub and one chrome node.
1. `make scale nodes=<num-nodes>` to scale the number of nodes for each browser.

## Misc
1. `http://localhost:4444/grid/console` to see your nodes.

## Config
1. You can override the default values passed to the environment variables in the *docker-compose.yml* file. Or,
1. You can modify the *.envrc* file directly.
1. You can also add different browser nodes by following the same docker-compose config for *selenium-chrome* and *selenium-firefox* but for a different selenium-node image.

## Local Setup
To use your selenium grid, you can reference the grid url `http://localhost:4444/wd/hub` with your test runner.

## Deps
1. [docker, docker-compose](https://docs.docker.com/docker-for-mac/install/)
1. [direnv](https://github.com/direnv/direnv)
