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
- [Docker環境でcomposerのimageつかってupdateしてみる - Qiita](https://qiita.com/yuya_sega/items/a8f2c3c58ae3762c0458)
- [ComposerをDockerコンテナで動かす - Qiita](https://qiita.com/PitPat/items/dc1ad09f7936b8825473)
