![EasePHP Framework Logo](https://raw.githubusercontent.com/VitexSoftware/Ease-PHP-Bricks/master/project-logo.png "Project Logo")

EasePHP Bricks
=================

Object oriented PHP Framework for easy&fast writing small/middle sized apps.

[![Latest Version](https://img.shields.io/github/release/VitexSoftware/Ease-PHP-Bricks.svg?style=flat-square)](https://github.com/VitexSoftware/Ease-PHP-Bricks/releases)
[![Software License](https://img.shields.io/badge/license-GPL-brightgreen.svg?style=flat-square)](https://github.com/VitexSoftware/Ease-PHP-Bricks/blob/master/LICENSE)
[![Build Status](https://img.shields.io/travis/VitexSoftware/Ease-PHP-Bricks/master.svg?style=flat-square)](https://travis-ci.org/VitexSoftware/Ease-PHP-Bricks)
[![Total Downloads](https://img.shields.io/packagist/dt/vitexsoftware/ease-bricks.svg?style=flat-square)](https://packagist.org/packages/vitexsoftware/ease-php-bricks)
[![Docker pulls](https://img.shields.io/docker/pulls/vitexsoftware/ease-bricks.svg)](https://hub.docker.com/r/vitexsoftware/ease-php-bricks/)
[![Downloads](https://img.shields.io/packagist/dt/vitexsoftware/ease-bricks.svg?style=flat-square)](https://packagist.org/packages/vitexsoftware/ease-php-bricks)
[![Latest stable](https://img.shields.io/packagist/v/vitexsoftware/ease-bricks.svg?style=flat-square)](https://packagist.org/packages/vitexsoftware/ease-php-bricks)

[![SensioLabsInsight](https://insight.sensiolabs.com/projects/4900ce8c-8619-4007-b2d6-0ac830064963/big.png)](https://insight.sensiolabs.com/projects/4900ce8c-8619-4007-b2d6-0ac830064963)


---

Bricks Included
===============

MainPageMenu
------------

Well framed large icons

![MainPageMenu](https://raw.githubusercontent.com/VitexSoftware/Ease-PHP-Bricks/master/MainPageMenu.png "Main Page Menu screenshot")

```php
$mpmenu = new \Ease\ui\MainPageMenu();
$mpmenu->addMenuItem('logo.png', 'Caption', 'https://url/');
```

TwitterBootstrap Switch
-----------------------

Ease support for http://bootstrapswitch.com/ 

![TWBSwitch](https://raw.githubusercontent.com/VitexSoftware/Ease-PHP-Bricks/master/TWBSwitch.png "Main Page Menu screenshot")

```php
new Ease\ui\TWBSwitch('swname', true, 1,['onText' => 'YES', 'offText' => 'NO']);
```

The **libjs-bootstrap-switch** package with requied js/css assets is already present in our repository https://www.vitexsoftware.cz/repo.php

Boolean LED
-----------

Show light or dark circle in given color.

![Boolean LED](https://raw.githubusercontent.com/VitexSoftware/Ease-PHP-Bricks/master/BooleanLED.png "Widget in green and red")

```php
new \Ease\ui\BooleanLED(false, 'green');
```



Installation
------------

To get Docker image:

    docker pull vitexsoftware/ease-bricks

For Debian, Ubuntu & friends please use repo:

    wget -O - http://v.s.cz/info@vitexsoftware.cz.gpg.key|sudo apt-key add -
    echo deb http://v.s.cz/ stable main > /etc/apt/sources.list.d/ease.list
    aptitude update
    aptitude install ease-bricks

In this case please add this to your app composer.json:

    "require": {
        "ease-bricks": "*"
    },
    "repositories": [
        {
            "type": "path",
            "url": "/usr/share/php/Ease",
            "options": {
                "symlink": true
            }
        }
    ]



Composer:
---------

    composer require vitexsoftware/ease-bricks

Links
=====

Homepage: https://www.vitexsoftware.cz/ease.php

GitHub: https://github.com/VitexSoftware/Ease-PHP-Bricks

Apigen Docs: https://www.vitexsoftware.cz/ease-php-bricks/
