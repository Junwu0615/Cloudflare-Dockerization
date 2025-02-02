<a href='https://github.com/Junwu0615/Cloudflare-Dockerization'><img alt='GitHub Views' src='https://views.whatilearened.today/views/github/Junwu0615/Cloudflare-Dockerization.svg'> 
<a href='https://github.com/Junwu0615/Cloudflare-Dockerization'><img alt='GitHub Clones' src='https://img.shields.io/badge/dynamic/json?color=success&label=Clone&query=count_total&url=https://gist.githubusercontent.com/Junwu0615/65175b78909744f87ef7330aba1945b4/raw/Cloudflare-Dockerization_clone.json&logo=github'> <br>
[![](https://img.shields.io/badge/Project-Cloudflare-blue.svg?style=plastic)](https://github.com/Junwu0615/Cloudflare-Dockerization) 
[![](https://img.shields.io/badge/Project-Docker-blue.svg?style=plastic)](https://github.com/Junwu0615/Cloudflare-Dockerization)
[![](https://img.shields.io/badge/Operating_System-Windows_10-blue.svg?style=plastic)](https://www.microsoft.com/zh-tw/software-download/windows10) <br>

<br>

## Dockerization

### *Directory Structure Diagram*
```commandline
Cloudflare-Dockerization/docker
  └── script
      ├── .env
      └── docker-compose.yaml
```

### *STEP.1　進入腳本路徑*
```bash
cd docker
```

### *STEP.2　新增檔案 : `./script/.env`*
```commandline
TUNNEL_TOKEN=<Your Auth Token>
```

### *STEP.3　安裝 docker-compose*
```bash
docker stack deploy -c script/docker-compose.yaml cloudflare-dockerization
```

### *STEP.4　檢視 docker service 清單*
```bash
docker service ls
```

### *STEP.5　查看專案 log 打印*
```bash
docker service logs -f cloudflare-dockerization_task
```

![jpg](/sample/00.jpg)

<br>

## Reference
- ### [cloudflare.com](https://dash.cloudflare.com/)
- ### [freenom.com](https://www.freenom.com/zu/index.html?lang=zu)
- ### [透過 Freenom 和 Cloudflare 取得免費域名](https://codelove.tw/@tony/post/1ay9Qa)
- ### [【白嫖Cloudflare】之免费内网穿透，让本地AI服务，触达全球](https://blog.csdn.net/u010522887/article/details/141621570)