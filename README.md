# docker-slate

## Run server

```sh
docker run \
-p 4567:4567 \
-v /path/to/doc-source:/app/source \
-v /path/to/build:/app/build \
sstc/slate
```

## Build

```sh
docker run \
-v /path/to/doc-source:/app/source \
-v /path/to/build:/app/build sstc/slate \
sh -c 'cp -nr source_orig/* source && exec bundle exec middleman build'
```

> see more at https://github.com/lord/slate/wiki/Docker#alternative-approach-with-ruby-25-alpine

