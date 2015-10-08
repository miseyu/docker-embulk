# docker-embulk
docker embulk

``` sh
docker build -t dockerfile/embulk --no-cache --rm=true ./
docker run -t -v ${PWD}:/work dockerfile/embulk  # help
```

## example

``` sh
$ docker run -t -v ${PWD}:/work dockerfile/embulk example ./try1
$ docker run -t -v ${PWD}:/work dockerfile/embulk guess ./try1/example.yml -o config.yml
```

## dry-run

``` sh
$ docker run -t -v ${PWD}:/work dockerfile/embulk preview config.yml
```

## run

``` sh
$ docker run -t -v ${PWD}:/work dockerfile/embulk run config.yml
```
