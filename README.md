# V2Ray Heroku

## Overview

Used to deploy V2Ray Websocket on Heroku.

**Heroku provides us with a free container service, we should not abuse it, so this project should not be used as a long-term use.**

**You can deploy more than two applications to achieve [Load Balancing](https://toutyrater.github.io/routing/balance2.html) to avoid a long-term high-traffic connection to an application and be judged as abuse by Heroku.**

**Heroku's network is not stable, please think twice before deploying.**

## Mirror

This image will not be blocked because it takes up a lot of resources.

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https%3A%2F%2Fgithub.com%2Fdopekid30%2Fv2ray-heroku-vmess)

## ENV settings

### UUID

`UUID`> `A UUID for the user to verify their identity when connecting`.

## Note

The WebSocket path is `/`.

`alterId` is `64`.

V2Ray will automatically install the latest version during deployment.

**For security reasons, unless you use CDN, please do not use a custom domain name, but use the second-level domain name assigned by Heroku to achieve V2Ray Websocket + TLS.**
