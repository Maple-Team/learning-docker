# Run Command

## Usage
```sh
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
```
## Option
Name, shorthand	| Description
|--|--|
|--name| Assign a name to the container 容器名 |
|--cpus|number of cpus|
|--env , -e|Set environment variables|
|--hostname , -h|		Container host name|
|--memory , -m	|	Memory limit|
|--net, --network	|	Connect a container to a network,容器编排|
|--volume , -v	|	Bind mount a volume 绑定到容器上|
|--expose	，-p	| Expose a port or a range of ports暴露端口|
|--detach , -d	|	Run container in background and print后台运行 |container ID
## Resouces
- [run reference](https://docs.docker.com/engine/reference/run/)