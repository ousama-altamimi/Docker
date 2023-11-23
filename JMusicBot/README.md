# JMusicBot Docker

<div align="left">
<a href="https://github.com/jagrosh/MusicBot/releases/latest"><img alt="github release" title="Basic code for JMusicBot" src="https://img.shields.io/github/v/release/jagrosh/MusicBot?style=for-the-badge&logo=github&logoColor=white&labelColor=2C4767&color=34567C"></a>
<a href="https://hub.docker.com/r/osama144/jmusicbot"><img alt="docker pulls" title="JMusicBot bot on Docker Hub" src="https://img.shields.io/docker/pulls/osama144/jmusicbot?style=for-the-badge&logo=docker&logoColor=white&labelColor=1155ba&color=236ad3"></a>
</div>
<br/>

Docker container for the latest version of [JMusicBot](https://github.com/jagrosh/MusicBot)

---

### 🐳 Docker CLI
```yaml
docker run -dit \  
  --name=JMusicBot \  
  -v $HOME/MusicBot:/data \
  --restart=unless-stopped \
  ghcr.io/ousama-altamimi/jmusicbot
```

### 🐳 Docker Compose

```yaml
version: "3"
services:
  jmusicbot:
    container_name: JMusicBot
    image: ghcr.io/ousama-altamimi/jmusicbot
    restart: unless-stopped
    volumes:
      - $HOME/MusicBot:/data
```
