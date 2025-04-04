# kong.gateway

Kong Gateway configuration for personal server

This repo uses [kongdecK](https://docs.konghq.com/deck/latest/) to build a kong gateway instance solely via configuration.

### Getting started

Go ahead and install the decK cli linked above.

Make changes to the `kong.yaml` file as needed.

Validate your changes with the following deck command

```bash
deck file validate kong.yaml
```

### Local Testing

Copy `.env.template` to `.env` modify if needed.

```bash
cp .env.template .env
```

Start up the docker instance

```bash
docker compose up -d
```

Tear down the docker instance

```bash
docker compose down
```

### Services Hosted in this Kong Gateway

| Service              | Url                                      |
| -------------------- | ---------------------------------------- |
| liteproxy.webservice | https://liteproxy.collinkleest.com/proxy |
| collinkleest.com     | https://collinkleest.com                 |
| fpl.app              | https://fpl.betlab.app/fpl.app/          |
