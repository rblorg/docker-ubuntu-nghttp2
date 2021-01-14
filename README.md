# Small size nghttp2 Docker image

Small size Docker based image for [nghttp2](https://nghttp2.org/).

It has the latest version of nghttp2 (v1.42.0).

Thank you for @centminmod for the inspiration.

There are other small images of nghttp2 but they use older versions ([centminmod/docker-ubuntu-nghttp2-minimal](https://github.com/centminmod/docker-ubuntu-nghttp2-minimal), [svagi/nghttp2](https://hub.docker.com/r/svagi/nghttp2)).

There is also [centminmod/docker-ubuntu-nghttp2](https://github.com/centminmod/docker-ubuntu-nghttp2) that is updated but is hugh (5.88GB).

I needed h2load with the arg `--connect-to` that was added in v1.40.0.
So I created this image.

I only tested it with h2load.

Location in Docker Hub: <https://hub.docker.com/r/erezarbell/nghttp2>

## Usage:
```
docker run --rm erezarbell/nghttp2 h2load ...
```
