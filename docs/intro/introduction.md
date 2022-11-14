# 官方简介

[![✍️ memos](https://raw.githubusercontent.com/usememos/memos/main/resources/logo-full.webp)](https://usememos.com)

An open-source, self-hosted memo hub for knowledge management and collaboration.

[![GitHub stars](https://img.shields.io/github/stars/usememos/memos)](https://github.com/usememos/memos/stargazers) [![Docker pull](https://img.shields.io/docker/pulls/neosmemo/memos.svg)](https://hub.docker.com/r/neosmemo/memos) ![Go report](https://goreportcard.com/badge/github.com/usememos/memos)

[Live Demo](https://demo.usememos.com/) • [Discuss in Telegram 👾](https://t.me/+-\_tNF1k70UU4ZTc9)

![demo](https://raw.githubusercontent.com/usememos/memos/main/resources/demo.webp)

### Features

* 🦄 Open source and free forever;
* 🚀 Support for self-hosting with `Docker` in seconds;
* 📜 Plain textarea first and support some useful markdown syntax;
* 👥 Collaborate and share with your teammates;
* 🧑‍💻 RESTful API for self-service.

### Deploy with Docker in seconds

#### Docker Run

```docker
docker run -d --name memos -p 5230:5230 -v ~/.memos/:/var/opt/memos neosmemo/memos:latest
```

Memos should be running at [http://localhost:5230](http://localhost:5230). If the `~/.memos/` does not have a `memos_prod.db` file, then memos will auto generate it.

#### Docker Compose

Example Compose YAML file: `docker-compose.yaml`.

If you want to upgrade the version of memos, use the following command.

```
docker-compose down && docker image rm neosmemo/memos:latest && docker-compose up -d
```

### Contribute

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are greatly appreciated. 🥰

See more in [development guide](https://github.com/usememos/memos/tree/main/docs/development.md).

### Community Products

* [Moe Memos](https://memos.moe/) - Third party client for iOS and Android
* [lmm214/memos-bber](https://github.com/lmm214/memos-bber) - Chrome extension
* [Rabithua/memos\_wmp](https://github.com/Rabithua/memos\_wmp) - Wechat miniprogram
* [qazxcdswe123/telegramMemoBot](https://github.com/qazxcdswe123/telegramMemoBot) - Telegram bot

### Star history

[![Star History Chart](https://api.star-history.com/svg?repos=usememos/memos\&type=Date)](https://star-history.com/#usememos/memos\&Date)
