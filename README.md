# Docker image with node and chrome (great with `puppeteer`)

## usage example

```Dockerfile
FROM itslooklike/node-chrome:1.0.1

COPY package.json yarn.lock ./
RUN yarn

COPY . .

CMD [ "yarn", "start" ]
```

<details>
  <summary>System info</summary>

```sh
docker build -t itslooklike/node-chrome:1.0.1 .
docker push itslooklike/node-chrome:1.0.1
```

</details>
