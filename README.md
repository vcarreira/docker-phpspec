# Phpspec container for Laravel

This is a [Docker](http://www.docker.com) image for [phpspec CLI](http://www.phpspec.net/) to be used with the [Laravel PHP Framework](http://laravel.com/).

An automated build for this repo is available on the [Docker Hub](https://registry.hub.docker.com/u/vcarreira/phpspec/).

This image works well with the below related images.

  - [vcarreira/nginx-php5-fpm](https://registry.hub.docker.com/u/vcarreira/nginx-php5-fpm)
  - [vcarreira/artisan](https://registry.hub.docker.com/u/vcarreira/artisan)
  - [vcarreira/composer](https://registry.hub.docker.com/u/vcarreira/composer)
  - [vcarreira/phpunit](https://registry.hub.docker.com/u/vcarreira/phpunit)

## Running phpspec commands
The container working directory is the volume ```/var/www```. You can run any phpspec command like this:

```
docker run -t --rm -v $(pwd):/var/www vcarreira/phpspec <phpspec args here>
```

---

:ok_hand: Happy Coding.

If you have any feedback or questions, feel free to contact me on Twitter with [@vcarreira](https://twitter.com/vcarreira) or email with [vitor.carreira@gmail.com](mailto:vitor.carreira@gmail.com).