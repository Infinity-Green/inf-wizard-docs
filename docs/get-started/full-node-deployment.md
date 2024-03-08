---
id: full-node-deployment
title: Full Node
---


Full node deployment of the Mind-chainblockchain.

## Requirements

* vCPUs >= 16
* Memory: at least 32GB
* Disk space
    * at least 1TB for the data directory ( recommend SSD ), solid-state drive(SSD), gp3, 8k IOPS, 250MB/S throughput, read latency <1ms. (for the best performance， it will need NVMe SSD)
    * data disk mount to /data
* Suggest m5zn.3xlarge instance type on AWS, c2-standard-16 on Google cloud.
* A broadband Internet connection with upload/download speeds of 5 megabyte per second.
* Linux os (one of them)
    * Ubuntu 20.04/22.04
    * CentOS 8.0+ / Rocky Linux 8.6 / Almalinux 8.6
    * Rocky Linux 9 / Almalinux 9
    * Debian 10/11
* curl or wget
* tar
* gzip




## Download && Installation

tap to see wizard [installation](./installation.md#installing-inf-wizard) command


## install core-node binery

```bash 
inf-wizard node install-inf
```



## Stake INF to become a Validator 

see the the commands for staking here [staking](./cli-commands.md#staking)

## Now generate keys and bootnode secrets from your node 




```shell
inf-wizard node init-secrets --data-dir node
```


### Get genesis file 

```bash 
inf-wizard node get-genesis
```


### Start the node server 

```shell
inf-wizard node start-inf-server
```


```
 $ inf-wizard node start-inf-server
  ___   _   _   _____          __        __  _                            _ 
 |_ _| | \ | | |  ___|         \ \      / / (_)  ____   __ _   _ __    __| |
  | |  |  \| | | |_     _____   \ \ /\ / /  | | |_  /  / _` | | '__|  / _` |
  | |  | |\  | |  _|   |_____|   \ V  V /   | |  / /  | (_| | | |    | (_| |
 |___| |_| \_| |_|                \_/\_/    |_| /___|  \__,_| |_|     \__,_|
                                                                            
Starting INF server...
INF server stdout: 

INF server stderr: 2024-03-08T06:29:51.463Z [INFO]  inf.server: Data dir: path=node

INF server stderr: 2024-03-08T06:29:51.487Z [INFO]  inf.blockchain: Current header: hash=0x21088e01bc44a0635545524f68938f9986130a164cb9b5cff814a008d3b51f96 number=581
2024-03-08T06:29:51.487Z [INFO]  inf.blockchain: genesis: hash=0xd8841f9a43ef9b10ce7bb0fdf20f43c02ebe82a25250d653bcb78f6dd6e98f4a

INF server stderr: 2024-03-08T06:29:51.487Z [INFO]  inf.server.ibft: validator key: addr=0x0745ca1150C412F28D48816c5250cf6160B4367D
2024-03-08T06:29:51.487Z [INFO]  inf.server: GRPC server running: addr=127.0.0.1:9632
2024-03-08T06:29:51.487Z [INFO]  inf.network: LibP2P server running: addr=/ip4/0.0.0.0/tcp/10001/p2p/16Uiu2HAkxLLVSptb6BQWm3X5YeQmqPSL6LSvpJtkMJ9koW5CoX8H

INF server stderr: 2024-03-08T06:29:51.488Z [INFO]  inf.server.jsonrpc: http server started: addr=0.0.0.0:8545
2024-03-08T06:29:51.488Z [INFO]  inf.txpool.event-manager: Added new subscription 222241586

INF server stderr: 2024-03-08T06:29:52.471Z [INFO]  inf.network: Peer connected: id=16Uiu2HAm1qdszjKn71TPzErmhT3oRCPD11UAC1Fj8gQZhnRMtx3e

INF server stderr: 2024-03-08T06:29:52.472Z [INFO]  inf.network: Peer connected: id=16Uiu2HAm4SHkeMXpLypiDuwCq3tFt9HL4kRMUqb12dmXWcjGFRkv

INF server stderr: 2024-03-08T06:29:52.473Z [INFO]  inf.network: Peer connected: id=16Uiu2HAmH8fZzqFri33kZtfEGKWFnKcbGPno77Ab7vEqbYnTxJgq

INF server stderr: 2024-03-08T06:29:52.473Z [INFO]  inf.network: Peer connected: id=16Uiu2HAm4NwvxUTkhC22NFQpDiTN1C5QtuegNfW7aS5MNx9TzeKo
```


`Congratulations you are started the node correctly and now you are a part of Infinity Green network` 


