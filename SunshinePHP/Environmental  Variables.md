# Environmental  Variables

Alena Holligan

[@alenaholligan](https://twitter.com/alenaholligan)

[Joind link](https://joind.in/talk/cf3cc)

[Examples](https://github.com/sketchings/example-env)

## What are environments?

Local, dev, QA, staging, production, etc

## What are environment variables?

* Tied to the environment
 * Not tied to a language
 * Not tied to an application
* Used for things that change based on the environment

## How can you set them up?

* Apache/Nginx (System wide or VHosts)
* Hosting company dashboard
* Docker
* .htaccess
* Composer package (.env)

## Security

Don't commit .env files.  Not really recommended for production

Use a secrets manager: [article](https://www.phparch.com/magazine/2019/06/how-to-tame-your-data/)
