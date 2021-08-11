## Setup

1. Create a `.env` file with the Outline environment variables and the add extras `OUTLINE_VERSION` and `OUTLINE_HOST` variables with the [Outline version](https://github.com/outline/outline/releases) and the hostname that the [Traefik](https://traefik.io/) will use to generate the [Let's Encrypt](https://letsencrypt.org/) security certificate.
   ```bash
   OUTLINE_VERSION=0.58.2
   OUTLINE_HOST=wiki.example.com
   
   # ... Outline config (see the docs: https://github.com/outline/outline)
   ```
   > The value of `OUTLINE VERSION` can be `latest` if you want the latest version of the app (not recommended).
1. Create an `acme.json` file:
   ```bash
   touch acme.json
   chmod 600 acme.json
   ```
1. Run the Docker containers with [Docker Compose](https://docs.docker.com/compose/):
   ```bash
   docker-compose up -d
   ```
