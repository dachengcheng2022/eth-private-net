### init account
```shell
docker run --rm -it \
  -v $(pwd)/data:/data \
  ethereum/client-go:v1.13 \
  account new --datadir /data
```

### run docker
```shell
docker compose up -d
```