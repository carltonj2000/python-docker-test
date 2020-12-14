# Containerized Python Development

```bash
docker build -t myimage .
docker run -d -p 5000:5000 myimage
# note got the slim image below for build but it failed running
docker build -t myimageslim -f Dockerfile.slim .
```

## History

The code in this repository is based on the
[Containerized Python Development](https://www.docker.com/blog/containerized-python-development-part-1/)
article.
