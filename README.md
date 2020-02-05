# KristianFJones/Docker-BindPlane

This is docker-compose stack that brings up a [Blue Medora BindPlane](https://bindplane.bluemedora.com/) collector server

## Usage

Clone this repo to your docker swarm manager or a docker container host inside of your management network.

Run the `./configureENVs.sh` script and fill in the values you get from [BindPlane New Colector](https://bindplane.bluemedora.com/collectors/new) in the Kubernetes config under the `data:` section. (You may need to fix/remove a new line in the output BindPlane.env file)

In thoery all you need to do is bring up the `docker-compose.yml` file

```
docker-compose up -d
```

I have not tested deploying as a stack to a docker swarm. I will update here once I have tested.

If you have any issues don't hesitate to contact me
