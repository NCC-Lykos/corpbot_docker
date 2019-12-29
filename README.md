## CorpBot docker container

This is a docker container of CorpBot.

## Docker pull

```
docker pull pavo/corpbot
```

## Example Intial Setup:

```
docker run -d --name corpbot -v /directorywhereyourfilesareloacted/token.txt:/home/docker/data/corpbot_docker/token.txt pavo/corpbot
```

## Example of converting from existing Bot:

```
docker run -d --name corpbot -v /directorywhereyourfilesareloacted/token.txt:/home/docker/data/corpbot_docker/token.txt -v /directorywhereyourfilesareloacted/Settings-Backup:/home/docker/data/corpbot_docker/Settings-Backup -v /directorywhereyourfilesareloacted/Settings.json:/home/docker/data/corpbot_docker/Settings.json pavo/corpbot
```

## Grabbing the Discord invite link:

Wait 1 minute after starting the container for the bot to fully initialize.

```
docker logs corpbot
```
