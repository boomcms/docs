---
currentMenu: getting-started
---

# Getting Started

## Requirements
As BoomCMS is based on [Laravel](http://www.laravel.com) it requires the same [PHP version and extensions](http://laravel.com/docs/5.0#installation) as Laravel.

In addition to Laravel's system requirements, BoomCMS also needs the imagick PHP extension.

## Installation
Installation is done via [Composer](https://getcomposer.org/)

```
composer create-project boomcms/boomcms <directory>
```

You will then need to ensure that the `storage` and `bootstrap/cache` directories are writable by your webserver.

After configuring your web server you can then go to the new Boom site in your browser to complete the installation.