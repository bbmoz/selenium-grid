# Selenium Grid

> Spin up your own selenium grid on a docker container with minimal configuration.

## Tasks
1. `make start` or `make` to start the grid with a hub, one chrome node, and one firefox node.
1. `make scale nodes={}` to scale the number of nodes for each browser.

## Misc
1. `http://localhost:4444/grid/console` to see your nodes.

## Config
1. You can override the default values passed to the environment variables in the *docker-compose.yml* file. Or,
1. You can modify the *.envrc* file directly.

## Local Setup
To use your selenium grid, you can reference the grid url `http://localhost:4444/wd/hub` with your test runner.
