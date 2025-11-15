# Claude-Code-DevContainer-Setup
Simple VSCode dev container setup for running Claude Code


This repo contains a `.devcontainer` folder. To use this in VSCode Dev Containers:
  - clone the repo and copy the `.devcontainer` folder to the root of your project directory
  - open the project folder in VSCode - it should prompt you to 'Reopen in Container'
  - This will run the .devcontainer/Dockerfile (using settings from .devcontainer/devcontainer.json)
  - The container will now be open and Terminal should verify you are the `devcon` user
      - The UID:GID should be 1000:1000 which lets it seamlessly work with WSL filesystem so new files created will be editable as normal
  - Claude Code should be installed and ready to use in VSCode in a fully sandboxed way
      - (You will need to sign in to Claude initially but only once, unless you rebuild the container)
