# Python dev environment

This is a simple python dev environment using docker.

## Requirements

- [Docker](https://www.docker.com/)
- [Visual Studio Code](https://code.visualstudio.com/)

## How to use

If you open this in visual studio code, it should give you a prompt to open the folder in a container. If not, you can open the command palette and search for `Remote-Containers: Open Folder in Container...` and select the folder.

## How to add packages

You can add packages to the `requirements.txt` file and then either run `pip install -r requirements.txt` in the terminal inside the container, or restart the container. This will install the packages in the container.

Note: `requirements` and `requirements-dev` are separated so that you can install packages that are only needed for development in the dev container. This is useful for things like linters and formatters.
