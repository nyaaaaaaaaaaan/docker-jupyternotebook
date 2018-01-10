# docker files
## it might be...
this image use CentOS. So maybe you have to pull centos.
```
docker pull centos
```

## how to use

### create image
```
docker build -t dev-python:1 .
```

### make work directory
```
mkdir notebooks
```

### run server as first time
```
docker run -d --name python -v `pwd`/notebooks:/opt/jupyter -p 8888:8888 dev-python:1
```

### start server
```
docker start dev-python:1
```

### access local server
plz access http://localhost:8888 for your browser.
