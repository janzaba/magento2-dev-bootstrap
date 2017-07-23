Fooman Magento 2 - Minimal Bootstrap
===================

This repository provides a barebones Magento 2 enviroment with a functional framework for development:
- instantiated ObjectManager
- working autogeneration of factories, proxies, etc 
- translations

The final aim for this project is to have tag 2.1.6 of this repository match Magento Opensource 2.1.6. with a fully 
automated creation of etc/di.xml, functions.php and composer.json based on the corresponding Magento version. 
This in turn means that until then commits and tags in this repository are subject to change.

### Installation Instructions via Composer

Add the below to your root composer.json file

    "repositories":[
      {
        "type":"vcs",
        "url":"http://github.com/fooman/magento2-dev-bootstrap"
      }
    ],

Magento's composer installer currently insists on the presence of the app/etc folder. Create it with

    mkdir -p app/etc

then run

    composer require-dev fooman/magento2-dev-bootstrap:dev-develop
