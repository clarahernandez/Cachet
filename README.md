<p align="center"><img src="https://demo.cachethq.io/img/cachet-logo.svg" width="50%"></p>

<p align="center">
<a href="https://styleci.io/repos/26730195/"><img src="https://styleci.io/repos/26730195/shield" alt="StyleCI"></a>
<a href="LICENSE"><img src="https://img.shields.io/badge/license-BSD3-brightgreen.svg?style=flat-square" alt="License"></a>
<a href="https://translate.cachethq.io/project/cachet"><img src="https://d322cqt584bo4o.cloudfront.net/cachet/localized.svg" alt="Localisation"></a>
<a href="https://github.com/CachetHQ/Cachet/releases"><img src="https://img.shields.io/github/release/cachethq/cachet.svg?style=flat-square" alt="Latest Stable Version"></a>
</p>

Cachet is a beautiful and powerful open source status page system.

## Overview

This project has a feature that adds the attribute 'team' to the Component model.

## Installation, Upgrades and Documentation

To install the project with Docker

1.  Clone the official repo of CachetHQ/Docker:

  ```shell
  git clone https://github.com/CachetHQ/Docker.git cachet-docker
  cd cachet-docker
  git tag -l
  git checkout $LATEST_TAG
  ```

2. Clone this repo of CachetHQ/Cachet here and do composer install:

  ```shell
  git clone https://github.com/clarahernandez/Cachet.git
  ```

3. Setup the Cachet project:

Note: This requires [Composer](https://getcomposer.org/) be installed on your Docker host.

 ```shell
cd Cachet
composer install
cp ../conf/.env.docker ./.env
cd ..
```

4. Edit the docker-compose.yml file to bind mount the repo as a volume:

  ```yaml
 cachet:
    volumes:
      - ./Cachet/:/var/www/html/
    ...
  ```

5. Build and run the container:

  ```shell
  docker-compose up
  ```

6. Open new terminal and run the following commands after getting container name via `docker ps`:

  ```shell
  docker exec -i cachetdocker_cachet_1  php artisan key:generate
  docker exec -i cachetdocker_cachet_1  php artisan app:install
  ```


You can find documentation at [https://docs.cachethq.io](https://docs.cachethq.io).

## Contributors

### Code Contributors

This project exists thanks to all the people who contribute. [[Contribute](CONTRIBUTING.md)].
<a href="https://github.com/CachetHQ/Cachet/graphs/contributors"><img src="https://opencollective.com/Cachet/contributors.svg?width=890&button=false" /></a>

### Financial Contributors

Become a financial contributor and help us sustain our community. [[Contribute](https://opencollective.com/Cachet/contribute)]

#### Individuals

<a href="https://opencollective.com/Cachet"><img src="https://opencollective.com/Cachet/individuals.svg?width=890"></a>

#### Organizations

Support this project with your organization. Your logo will show up here with a link to your website. [[Contribute](https://opencollective.com/Cachet/contribute)]

<a href="https://opencollective.com/Cachet/organization/0/website"><img src="https://opencollective.com/Cachet/organization/0/avatar.svg"></a>
<a href="https://opencollective.com/Cachet/organization/1/website"><img src="https://opencollective.com/Cachet/organization/1/avatar.svg"></a>
<a href="https://opencollective.com/Cachet/organization/2/website"><img src="https://opencollective.com/Cachet/organization/2/avatar.svg"></a>
<a href="https://opencollective.com/Cachet/organization/3/website"><img src="https://opencollective.com/Cachet/organization/3/avatar.svg"></a>
<a href="https://opencollective.com/Cachet/organization/4/website"><img src="https://opencollective.com/Cachet/organization/4/avatar.svg"></a>
<a href="https://opencollective.com/Cachet/organization/5/website"><img src="https://opencollective.com/Cachet/organization/5/avatar.svg"></a>
<a href="https://opencollective.com/Cachet/organization/6/website"><img src="https://opencollective.com/Cachet/organization/6/avatar.svg"></a>
<a href="https://opencollective.com/Cachet/organization/7/website"><img src="https://opencollective.com/Cachet/organization/7/avatar.svg"></a>
<a href="https://opencollective.com/Cachet/organization/8/website"><img src="https://opencollective.com/Cachet/organization/8/avatar.svg"></a>
<a href="https://opencollective.com/Cachet/organization/9/website"><img src="https://opencollective.com/Cachet/organization/9/avatar.svg"></a>
