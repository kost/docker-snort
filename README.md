# k0st/snort

A Docker container for Snort (10.18 MB).

Image is based on the [gliderlabs/alpine](https://registry.hub.docker.com/u/gliderlabs/alpine/) base image

## Docker image size

[![Latest](https://badge.imagelayers.io/k0st/snort.svg)](https://imagelayers.io/?images=k0st/snort:latest 'latest')


## Docker image usage

```
docker run k0st/snort [Snort options]
```

## Examples

Process pcap file called sniff.pcap using snort:

```
docker run -v /path/to/pcap/dir:/work:rw k0st/snort -r sniff.pcap
```

Display snort version and do not keep container:

```
docker run --rm=true k0st/snort --version
```

Display help and do not keep container:

```
docker run --rm=true k0st/snort --help
```


