# Selenium Grid CC

> Spin up your own selenium grid on a docker container with minimal configuration.

## Tasks
1. `make start` or `make` to start the grid with a hub, one chrome node, and one firefox node.
1. `make scale nodes=<num-nodes>` to scale the number of nodes for each browser (default is 1).

## Misc
1. `http://localhost:4444/grid/console` to see your nodes.
1. `docker logs selenium-hub` to see hub logs. To tail, use `-f`.

## Config
1. You can override the default values passed to the environment variables in the *docker-compose.yml* file. Or,
1. You can modify the *.envrc* file directly.
1. To add different browser nodes, follow the docker-compose config for *selenium-chrome* or *selenium-firefox*.

## Local
To use your selenium grid, reference the grid url `http://localhost:4444/wd/hub` with your test runner.

