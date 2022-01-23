# Docker image with node, pnpm, chrome (great with `puppeteer`)

https://hub.docker.com/repository/docker/itslooklike/node-chrome

## usage example

```Dockerfile
FROM itslooklike/node-chrome:1.2.0

COPY pnpm.json pnpm-lock.yaml ./
RUN pnpm i

COPY . .

CMD [ "pnpm", "start" ]
```

<details>
  <summary>System info</summary>

```sh
# release container
docker build -t itslooklike/node-chrome:1.2.0 .
docker push itslooklike/node-chrome:1.2.0
```

</details>
