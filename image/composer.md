# Composer

## 使い方
### docker-compose.yml
```yml
version: "3.8"

services:
  composer:
    image: composer
    command: "composer install"
    volumes:
    - ./:/app
```

### コマンド
```bash
docker-compose run composer composer require --dev phpunit/phpunit
```


## 参考
- [環境を汚さずに Composer を使いたい - Qiita](https://qiita.com/SnowCait/items/e70ec1a7d365b490c2b2)
- [SnowCait/docker-compose-composer-example: Composer container usage.](https://github.com/SnowCait/docker-compose-composer-example)
- [Docker環境でcomposerのimageつかってupdateしてみる - Qiita](https://qiita.com/yuya_sega/items/a8f2c3c58ae3762c0458)
- [ComposerをDockerコンテナで動かす - Qiita](https://qiita.com/PitPat/items/dc1ad09f7936b8825473)
