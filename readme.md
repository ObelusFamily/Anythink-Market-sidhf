# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_

### Docker setup

* `git clone` the repo with the link from GitHub --> git@github.com:ObelusFamily/Anythink-Market-sidhf.git
    * Ensure that SSH is setup to work with your env and Github
Install docker on WSL for two layer virtualisation on Win10 --> https://docs.docker.com/desktop/windows/wsl/
* Enable docker integration with your chosen linux distro on WSL2 
    - Docker Desktop-Settings-Resources
    - Tick WSL2 Integration & restart docker / Wsl
* Verify succsefful docker installation via `docker -v` and `docker-compose -v`
* Start Docker container by navigation to the path where the git repo is cloned
    * Start the container by `docker-compose up`
    * Navigate to the backend and frontend urls:
        * http://localhost:3000/api/ping
        * http://localhost:3001/register
* Well done! If you're able to create a user on the FrontEnd then everything works as intended.