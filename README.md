# Dokku Prometheus nodeexporter

[Prometheus nodeexporter](https://github.com/prometheus/node_exporter) plugin for [dokku](https://github.com/progrium/dokku) >= 0.4.0

Simple plugin that adds a `nodeexporter` entry to the Dokku's menu to start/stop the service.

Note that the container needs to run in privilege modes. Host volumes are mounted read-only.

## Installation

On the Dokku server run the following:
```
sudo dokku plugin:install https://github.com/mtarnovan/dokku-nodeexporter nodeexporter
```

## Usage

```
dokku nodeexporter # Show the status of nodeexporter
dokku nodeexporter:start # Starts nodeexporter
dokku nodeexporter:stop # Stop nodeexporter
```
