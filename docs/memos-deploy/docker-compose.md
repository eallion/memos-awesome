# Docker Compose

官方提供的 `docker-compose.yml`

[https://github.com/usememos/memos/blob/main/docker-compose.yaml](https://github.com/usememos/memos/blob/main/docker-compose.yaml)

{% code title="docker-compose.yml" %}
```yaml
version: "3.0"
services:
  memos:
    image: neosmemo/memos:latest
    container_name: memos
    restart: always
    volumes:
      - ~/.memos/:/var/opt/memos
    ports:
      - 5230:5230
```
{% endcode %}

启动：

```bash
docker compose up -d
```

升级：

```bash
docker compose pull && docker compose up -d --force-recreate
```
