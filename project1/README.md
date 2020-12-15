# Containerized Python Development

```bash
pushd backend; docker build -f Dockerfile -t backend . ; popd
pushd frontend; docker build -f Dockerfile -t frontend . ; popd
docker stack deploy project1 --compose-file docker-compose.yaml
docker stack remove project1
# debug by running container one at a time
docker run -d -p 80:80 frontend
```

## History

The code in this repository is based on the
[Containerized Python Development](https://www.docker.com/blog/containerized-python-development-part-2/)
article.
