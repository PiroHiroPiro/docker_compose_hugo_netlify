# HUGO + Netlify Docker template

This is a Docker template that provides an environment with [HUGO](https://gohugo.io/).

## Requirement

- [git](https://git-scm.com/)
- [Docker](https://www.docker.com/)
  - docker-compose

## Develop

Run local:

```console
$ docker-compose up
```

Go to `http://localhost:1313` and you'll see the website.

## Deploy

Deploy to [Netlify](https://www.netlify.com/):

```console
$ git push origin master
```

## Install

Clone repository:

```console
$ git clone https://github.com/PiroHiroPiro/docker_template_hugo_netlify.git
$ cd docker_template_hugo_netlify
```

Build images:

```console
$ docker-compose build
```

Create a new site:

```console
$ docker-compose run hugo hugo new site .
```

Choose [Hugo themes](https://themes.gohugo.io/) and add a theme:

```console
$ git submodule add https://github.com/budparr/gohugo-theme-ananke.git site/themes/ananke
```

## How to use

Create new Post:

```console
$ docker-compose run hugo hugo new posts/initial-post.md
```

Update themes:

```console
$ git submodule update --remote
```

## Author

[Hiroyuki Nishizawa](https://github.com/PiroHiroPiro)
