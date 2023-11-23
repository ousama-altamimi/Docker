# JMusicBot Docker
![GitHub release (with filter)](https://img.shields.io/github/v/release/jagrosh/MusicBot?style=for-the-badge&logo=github&logoColor=white&labelColor=2C4767&color=34567C) ![Docker Pulls](https://img.shields.io/docker/pulls/osama144/jmusicbot?style=for-the-badge&logo=docker&logoColor=white&labelColor=1155ba&color=236ad3&link=https%3A%2F%2Fhub.docker.com%2Fr%2Fosama144%2Fjmusicbot)



Docker container for the latest version of [JMusicBot](https://github.com/jagrosh/MusicBot)

---

### Docker CLI
```yaml
docker run -dit \  
  --name=JMusicBot \  
  -v $HOME/MusicBot:/data \
  --restart=unless-stopped \
  osama144/jmusicbot
```

### Docker Compose

```yaml
version: "3"
services:
  jmusicbot:
    container_name: JMusicBot
    image: osama144/jmusicbot
    restart: unless-stopped
    volumes:
      - $HOME/MusicBot:/data
```
