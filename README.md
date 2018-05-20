# WordPress test environment for PHPUnit

## About

Initialize a [Vagrant](https://www.vagrantup.com/) box based on [Laravel Homestead.](http://laravel.com/docs/5.1/homestead)

Test WordPress plugins

## Requirements

- [Vagrant](http://www.vagrantup.com/downloads.html)
- [VirtualBox 5.x](https://www.virtualbox.org/wiki/Downloads)
- PHP 5.6+
- [Composer](https://getcomposer.org/doc/00-intro.md)

## Get started

### Initial setup

Clone the repo and go to your cloned directory and install composer dependencies by running following command:

```
composer install
```

### Setting Your SSH Key
You will need to have ssh keys for accessing virtual server. On Mac and Linux, you can create an SSH key pair using the following command:

```
ssh-keygen -t rsa -C "you@wordpress"
```

### Run vagrant box

To run vagrant box type:

```
vagrant up
```

This shall create a new instance of Ubuntu 18.04 with included softwares.

To ssh new instance, run following command:

```
vagrant ssh
```

### Homestead.yaml

Homestead.yaml comes with several configurations. You can map any local directory to virtual server and also configure custom domain.

To get more info about homestead, visit [Laravel Homestead](http://laravel.com/docs/5.1/homestead)
