# docker-multichain

This is Bloomen.io Multichain demo repository based on kunstmaan (https://github.com/Kunstmaan/docker-multichain) github repository.

## Images

* [kunstmaan/base-multichain](https://hub.docker.com/r/kunstmaan/base-multichain/): A base Ubuntu with the latest Multichain deamon installed
* [kunstmaan/master-multichain](https://hub.docker.com/r/kunstmaan/master-multichain/): Based on the "base" image running a master node, creates a blockchain and runs it. *Important: only for development since any node can connect, anyone can administer and the RPC interface is open to all.*
* [kunstmaan/node-multichain](https://hub.docker.com/r/kunstmaan/node-multichain/): Based on the same "base" image and connects to the master node
* [kunstmaan/explorer-multichain](https://hub.docker.com/r/kunstmaan/explorer-multichain/): A node with the Multichain explorer installed
* [worldline-spain/multichain-web-demo](https://github.com/worldline-spain/multichain-web-demo): A node with the Multichain web demo customized for bloomen.io

## Running the cluster

Use this [docker-compose.yml](https://github.com/bloomenio/docker-multichain/blob/master/docker-compose.yml) and run:

```
sudo docker-compose up
```

## Services

### Multichain web demo

Accessible through port 8080 (http://localhost:8080)

### Multichain explorer

Accessible through port 2750 (http://localhost:2750)
 

