# Multi webapp for YunoHost

[![Integration level](https://dash.yunohost.org/integration/multi_webapp.svg)](https://ci-apps.yunohost.org/jenkins/job/multi_webapp%20%28Community%29/lastBuild/consoleFull)  
[![Install Multi webapp with YunoHost](https://install-app.yunohost.org/install-with-yunohost.png)](https://install-app.yunohost.org/?app=multi_webapp)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allow you to install Multi webapp quickly and simply on a YunoHost server.  
If you don't have YunoHost, please see [here](https://yunohost.org/#/install) to know how to install and enjoy it.*

## Overview

Blank web app container made to be used with a non yet packaged web application.
This application can be installed a multiple times.

**Shipped version:** NA

## Screenshots

## Configuration

## Documentation

 * YunoHost documentation: There no other documentations, feel free to contribute.

## YunoHost specific features

#### Multi-users support

#### Supported architectures

* Tested on x86_64

## Limitations

## Additionnal informations

A directory will be created for your application in `/var/www/webapp_USER/DOMAIN_PATH`. Your application shall be put inside.
You can find a standard nginx configuration in `/etc/nginx/conf.d/DOMAIN.d/webapp_DOMAIN_PATH.conf` and a standard php config in `/etc/php5/fpm/pool.d/webapp_DOMAIN_PATH.conf` and `/etc/php5/fpm/conf.d/20-webapp_DOMAIN_PATH.ini`.
If you ask for a database, your credentials will be in the file `/var/www/webapp_USER/DOMAIN_PATH/db_info.txt`

## Links

 * Report a bug: https://github.com/YunoHost-Apps/multi_webapp_ynh/issues
 * YunoHost website: https://yunohost.org/

---

Developers infos
----------------

Please do your pull request to the [testing branch](https://github.com/YunoHost-Apps/multi_webapp_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/multi_webapp_ynh/tree/testing --verbose
or
sudo yunohost app upgrade multi_webapp -u https://github.com/YunoHost-Apps/multi_webapp_ynh/tree/testing --verbose
```
