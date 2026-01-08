### init account
```shell
docker run --rm -it \
  -v $(pwd)/data:/data \
  ethereum/client-go:alltools-latest \
  geth account new --datadir /data
```

### init genesis
```shell
docker run --rm \
  -v $(pwd)/data:/data \
  -v $(pwd)/genesis.json:/genesis.json \
  ethereum/client-go:alltools-latest \
  geth --datadir /data init /genesis.json
```

### run docker
```shell
docker compose up -d
```