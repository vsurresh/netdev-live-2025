


Steps

1. Initialize uv project



```shell
uv init devnet-live-2025
cd devnet-live-2025
uv add infrahub-sdk --extra all
```

```
    # "infrahub-sdk[all] @ git+https://github.com/opsmill/infrahub-sdk-python.git@dga-20250330-object-cmd",
```

2. Create project structure

```shell
mkdir schemas
mkdir data
mkdir templates
mkdir tests
```

3. Start infrahub

```shell
curl https://infrahub.opsmill.io | docker compose -p infrahub -f - up -d
```

```shell
curl https://infrahub.opsmill.io > docker-compose.yaml
docker compose up -d
```
```shell
docker compose down -v
```

4. Explore the schema


5. Configure Infrahubctl
```
source .venv/bin/activate
```

```
export INFRAHUB_USERNAME=admin
export INFRAHUB_PASSWORD=infrahub
export INFRAHUB_ADDRESS=http://localhost:8000
```

```
infrahubctl info
```

