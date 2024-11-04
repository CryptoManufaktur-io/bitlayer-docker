# Overview

Docker Compose for Bitlayer rollup

`cp default.env .env`, then `nano .env` and adjust values

This repo does not support Bitlayer on Sepolia at present

Meant to be used with [central-proxy-docker](https://github.com/CryptoManufaktur-io/central-proxy-docker) for traefik
and Prometheus remote write; use `:ext-network.yml` in `COMPOSE_FILE` inside `.env` in that case.

If you want the op-geth RPC ports exposed locally, use `rpc-shared.yml` in `COMPOSE_FILE` inside `.env`.

The `./bitlayerd` script can be used as a quick-start:

`./bitlayerd install` brings in docker-ce, if you don't have Docker installed already.

`cp default.env .env`

`nano .env` and adjust variables as needed

`./bitlayerd up`

To update the software, run `./bitlayerd update` and then `./bitlayerd up`

This is Bitlayer Docker v1.0.0
