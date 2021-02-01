# Docker

Getting started with Docker:

```bash
docker run -d -p 80:80 docker/getting-started
```

`-d` - run the container in detached mode (in the background)
`-p` 80:80 - map port 80 of the host to port 80 in the container (`local:container`)

`-dp` could be combined:

```bash
docker run -dp 80:80 docker/getting-started
```

## Dockerfile

`FROM` is the basic image.

Build the image:

```bash
docker build -t hello-world .
docker run -dp 3000:3000 hello-world
http :3000
# `-t` is the tag of the image
# `.` indicates the `Dockerfile`'s directory
```
