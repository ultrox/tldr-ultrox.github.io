# docker

> Manage Docker containers and images.

- New interactive container with name supercool from image ubuntu 

`docker run -it --name {{supercool}} {{ubuntu}}`

- Start a container from an image, with a custom name:

`docker container run --name={{container_name}} {{image}}`

- New detached container with maped ports

`docker run -td --name {{supercool}} -p 8080:8080 {{ubuntu}}`

- List currently running docker containers:

`docker container {{start|stop}} {{container_name}}`

- Start a container from an image and get a shell inside of it:

`docker container run -it {{image}} bash`

- Run a command inside of an already running container:

`docker container exec {{container_name}} {{command}}`

- Fetch and follow the logs of a container:

`docker container logs -f {{container}}`

- Rename container

`docker rename {{oldname}} {{newname}}`
