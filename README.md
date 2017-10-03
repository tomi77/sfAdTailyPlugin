# AdTaily integration Plug-in

The `sfAdTailyPlugin` offers the integrate with [AdTaily](http://www.adtaily.com/).

[![StyleCI](https://styleci.io/repos/49574524/shield?style=plastic&branch=master)](https://styleci.io/repos/49574524)

## Instalation

  * Install the plugin:

    ~~~sh
    $ symfony plugin:install sfAdTailyPlugin
    ~~~

  * Activate helper:

    ~~~php
    use_helper('AdTaily');
    ~~~

    or in `settings.yml`

    ~~~yaml
    all:
      standard_helpers: [..., AdTaily]
    ~~~

  * Clear cache

    ~~~sh
    $ symfony cc
    ~~~

## Configuration

  * Configuration is done in your application's app.yml file:

    ~~~yaml
    all:
      ad_taily_plugin:
        enabled: true
        code:    xxxxxx
    ~~~

## Use

Insert in your template:

~~~html
<?php at_insert_ad_taily_ad() ?>
~~~
