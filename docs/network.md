# docker network
应用场景：容器之间相互访问
## 类型
- bridge
- host 宿主机共享，性能最好，但端口会有冲突的问题
- none
- ovelay
- macvlan
## 网络模型架构
TODO
## Usage
```sh
 docker network COMMAND
 ```
 ## docker network create
 ```sh
 Usage:  docker network create [OPTIONS] NETWORK

Create a network

Options:
  -d, --driver string        Driver to manage the Network (default "bridge")
      --gateway strings      IPv4 or IPv6 Gateway for the master subnet
      --ip-range strings     Allocate container ip from a sub-range
      --subnet strings       Subnet in CIDR format that represents a
                             network segment
 ```

## TODO
- 理解linux的网络模型、网卡等