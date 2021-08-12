nginx-vod-module-container
=======================
This is a non-root user container image for Nginx VOD module 

This repository contains a Dockerfile for building nginx with [Kaltura's
vod-module](https://github.com/kaltura/nginx-vod-module).

The Dockerfile is desgined for a non-root user container image and derived from [NYTimes nginx-vod-module-docker](https://github.com/nytimes/nginx-vod-module-docker) 

Building locally
----------------

This repository uses Docker's multi-stage builds, therefore building this image
requires Docker 19.03 or higher. Given that you have all the required
dependencies, building the image is as simple as running a ``docker build``:

```
docker build -t smccloudarchitect/nginx-vod-module .
```
