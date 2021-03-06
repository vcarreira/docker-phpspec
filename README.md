# Phpspec container for Laravel

This is a [Docker](http://www.docker.com) image for [phpspec CLI](http://www.phpspec.net/) to be used with the [Laravel PHP Framework](http://laravel.com/).

An automated build for this repo is available on the [Docker Hub](https://registry.hub.docker.com/u/vcarreira/phpspec/).

This image works well when used with the [Docker Laravel](https://github.com/vcarreira/docker-laravel) multi-container solution.

## Images used by [Docker Laravel](https://github.com/vcarreira/docker-laravel)
  - [vcarreira/nginx-php7-fpm](https://registry.hub.docker.com/u/vcarreira/nginx-php7-fpm)
  - [vcarreira/redis](https://registry.hub.docker.com/u/vcarreira/redis)
  - [vcarreira/composer](https://registry.hub.docker.com/u/vcarreira/composer)
  - [vcarreira/artisan](https://registry.hub.docker.com/u/vcarreira/artisan)
  - [vcarreira/node](https://registry.hub.docker.com/u/vcarreira/node)
  - [vcarreira/phpspec](https://registry.hub.docker.com/u/vcarreira/phpspec)
  - [vcarreira/phpunit](https://registry.hub.docker.com/u/vcarreira/phpunit)

## Running phpspec commands
The container working directory is the volume ```/var/www```. You can run any phpspec command like this:

```
docker run -t --rm -v $(pwd):/var/www vcarreira/phpspec <phpspec args here>
```

---

:ok_hand: Happy Coding.

If you have any feedback or questions, feel free to contact me on Twitter with [@vcarreira](https://twitter.com/vcarreira) or email with [vitor.carreira@gmail.com](mailto:vitor.carreira@gmail.com).
