## Setup

1. Create a `.env` file with the Outline environment variables and the a `TRAEFIK_HOST` variable with the hostname that the Traefik will use to generate the Let's Encrypt security certificate.
1. Create `acme.json` file:

  `touch acme.json && chmod 600 acme.json`
1. Run the Docker containers with `docker-compose`:

  `docker-compose up -d`