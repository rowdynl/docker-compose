# Docker compose
All docker compose files for my homelab.

## Structure
I've created a sub folder per stack. Each has a symbolic link to the .env file in the root folder.

```
compose
 .env
  |- code-server
   | - docker-compose
   | - .env --> ../.env
  |- plex
   | - docker-compose
   | - .env --> ../.env
 |- etc
```

## .env example
Example .env file
```
TZ=Europe/Amsterdam
PUID=1000
PGID=100

# CODE SERVER
CODE_SERVER_HOMEASSISTANT_URL=http://192.168.178.100:8123
CODE_SERVER_HOMEASSISTANT_TOKEN=a-pat-from-has
CODE_SERVER_PASSWORD=password-for-code-server-to-be-replaced-by-authentic
```