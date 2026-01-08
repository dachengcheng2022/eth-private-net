### init account
```shell
docker run --rm -it \
  -v $(pwd)/data:/data \
  ethereum/client-go:alltools-latest \
  geth account new --datadir /data
```

### run docker
```shell
docker compose up -d
```