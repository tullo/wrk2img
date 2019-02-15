# wrk2img

Generate latency graph from benchmark files produces with [wrk2](https://hub.docker.com/r/tullo/wrk2)

## Build image

`DOCKER_BUILDKIT=1 docker build -t wrk2image .`

## Example Usage

1. Get inside a container
    `docker run -it -v $(pwd):/data wrk2image`
1. Generate a graphical representation of an input file
    `cat input/R18000 | wrk2img output/latency.png`