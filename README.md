# easy-smart-contract

#### Docker command

```
docker run -d --name ethereum -v ~/ethereum:/root \
-p 8545:8545 -p 30303:30303 \
ethereum/client-go \
--ipcapi "admin, db, eth, debug, miner, net, shh, txpool, personal, web3"  \
--rpc --rpccorsdomain "*"  \
--rpcapi "db, eth, net, web3, personal"  \
--rpcport "8545" \
--port "6666" \
--networkid "9487" \
--nodiscover 
```

```
docker exec -it ethereum /geth attach
```