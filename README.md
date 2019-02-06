# Vagrant Box - LAMP stack - PHP 5.5.9

- Ubuntu 14.04.5 LTS
- Apache 2.4.7
- MySQL 5.5.62
- PHP 5.5.9
- phpMyAdmin 4.0.10

## Installation

- Install [VirtualBox](https://www.virtualbox.org/)
- Install [Vagrant](https://www.vagrantup.com/)
- `git clone http://github.com/rahamatjahan/lamp-php55.git`
- `cd lamp-php55`
- `vagrant up`
- Put your code inside the `public` folder
- Visit [http://192.168.55.90](http://192.168.55.90)
- phpMyAdmin [http://192.168.55.90/phpmyadmin](http://192.168.55.90/phpmyadmin) (username: root | password: password)

## Configuration

- Change IP and synced folder inside `Vagrantfile`
- Change MySQL username, password and database name inside `bootstrap.sh`
- Run `vagrant reload` to allow changes to take effect