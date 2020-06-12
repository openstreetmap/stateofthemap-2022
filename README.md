# State of the Map 2020 Website

## Local installation

### Install Jekyll

See http://jekyllrb.com/docs/installation/

### View locally

* `git clone git@github.com:openstreetmap/stateofthemap-2020.git`
* `cd stateofthemap-2020`
* `jekyll serve -wl`
* Point your browser to `http://localhost:4000/`

## Docker

Alternatively you can use Docker to install Jekyll and to serve the site within a container.

### Using docker-compose

* [Install docker-compose](https://docs.docker.com/compose/install/)
* `git clone git@github.com:openstreetmap/stateofthemap-2020.git`
* `cd stateofthemap-2020`
* `docker-compose up --build`
* Point your browser to `http://localhost:4000/`

Alternatively if you are using docker-machine, replace localhost with the IP address from `docker-machine ip`

## Contributing

### Code Style

Please adhere to the code style rules in the supplied `.editorconfig` file. Instructions for [editors/IDEs](https://editorconfig.org/#download).
