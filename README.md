# GoMore Boilerplate
GoMore (Golang, Docker, React, Mongodb) boilerplate.

## Features
- [x] Docker containers config
- [ ] React Redux Boilerplate
- [x] Golang Mux boilerplate
- [ ] Mongodb setup
- [ ] CD/CI Jenkins integration

## Benifits
- Anyone can contribute to your project locally without having to setup/install GOPATH, Mongodb, node etc
- Dev enviroment is the same as production enviroment
- Quickly get your GoMore project off the ground

## Getting started:
* download [docker-compose](https://docs.docker.com/compose/install/) if not already installed
Then run the following commands:

```bash
$ git clone https://github.com/hugominas/gomore.git yourAddDir.
$ docker-compose up
```
Then you can open the React frontend at localhost:3000 and the RESTful GoLang API at localhost:5000

Changing any frontend (React) code locally will cause a hot-reload in the browser with updates and changing any backend (GoLang) code locally will also automatilly update any changes.

Then to build production images run:
```bash
$ docker build ./api --build-arg app_env=production
$ docker build ./frontend --build-arg app_env=production
$ docker build ./db
```
