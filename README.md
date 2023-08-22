# HUGO + Netlify Docker template

This is a Docker template that provides an environment with [HUGO](https://gohugo.io/).

## Requirement

- [git](https://git-scm.com/)
- [Docker](https://www.docker.com/)
  - docker-compose

## Develop

Run local:

```shell
$ docker-compose up
```

Go to `http://localhost:1313` and you'll see the website.

## Deploy

Deploy to [Netlify](https://www.netlify.com/):

```shell
$ git push origin main
```

## Install

Clone repository:

```shell
$ git clone --recursive https://github.com/PiroHiroPiro/docker_template_hugo_netlify.git
$ cd docker_template_hugo_netlify
```

Build images:

```shell
$ docker-compose build
```

Create a new site:

```shell
$ docker-compose run hugo hugo new site .
```

Choose [Hugo themes](https://themes.gohugo.io/) and add a theme:

```shell
$ git submodule add https://github.com/budparr/gohugo-theme-ananke.git site/themes/ananke
```

## How to use

Create new Post:

```shell
$ docker-compose run hugo hugo new posts/initial-post.md
```

Update themes:

```shell
$ git submodule update --remote
```

## Author

[Hiroyuki Nishizawa](https://github.com/PiroHiroPiro)
