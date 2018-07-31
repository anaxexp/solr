# Apache Solr Docker Container Image

[![Build Status](https://travis-ci.org/anaxexp/solr.svg?branch=master)](https://travis-ci.org/anaxexp/solr)
[![Docker Pulls](https://img.shields.io/docker/pulls/anaxexperience/solr.svg)](https://hub.docker.com/r/anaxexperience/solr)
[![Docker Stars](https://img.shields.io/docker/stars/anaxexperience/solr.svg)](https://hub.docker.com/r/anaxexperience/solr)
[![Docker Layers](https://images.microbadger.com/badges/image/anaxexperience/solr.svg)](https://microbadger.com/images/anaxexperience/solr)

## Docker Images

❗️For better reliability we release images with stability tags (`anaxexperience/solr:7-X.X.X`) which correspond to [git tags](https://github.com/anaxexp/solr/releases). We strongly recommend using images only with stability tags. 

* All images are based on Alpine Linux
* Base image: [solr](https://hub.docker.com/r/_/solr)
* [Travis CI builds](https://travis-ci.org/anaxexp/solr) 
* [Docker Hub](https://hub.docker.com/r/anaxexperience/solr)

[_(Dockerfile)_]: https://github.com/anaxexp/solr/tree/master/Dockerfile

Supported tags and respective `Dockerfile` links:

* `7.4`, `7`, `latest` [_(Dockerfile)_]
* `7.3` [_(Dockerfile)_]
* `7.2` [_(Dockerfile)_]
* `7.1` [_(Dockerfile)_]
* `6.6`, `6` [_(Dockerfile)_]
* `5.5`, `5` [_(Dockerfile)_]
* `5.4` [_(Dockerfile)_]

## Environment Variables

| Variable    | Default Value |
| ----------- | ------------- |
| `SOLR_HEAP` | `1024m `      |

## Orchestration actions

Usage:
```
make COMMAND [params ...]

commands:
    create (default) core [host config_set instance_dir] 
    init [host] 
    ping core [host]
    reload core [host]
    delete core [host]
    check-ready [host max_try wait_seconds]
 
default params values:
    host localhost
    config_set data_driven_schema_configs (or _default in newer versions)
    max_try 1
    wait_seconds 1
    delay_seconds 0
```

## Deployment

Deploy Solr to your server via [![Wodby](https://www.google.com/s2/favicons?domain=anaxexp.io) Wodby](https://cloud.anaxexp.io/stackhub/dc8074a9-f27d-44a8-8f88-5922b4e16d2f).
