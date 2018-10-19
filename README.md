<!--
#                                 __                 __
#    __  ______  ____ ___  ____ _/ /____  ____  ____/ /
#   / / / / __ \/ __ `__ \/ __ `/ __/ _ \/ __ \/ __  /
#  / /_/ / /_/ / / / / / / /_/ / /_/  __/ /_/ / /_/ /
#  \__, /\____/_/ /_/ /_/\__,_/\__/\___/\____/\__,_/
# /____                     matthewdavis.io, holla!
#
#-->

[![Clickity click](https://img.shields.io/badge/k8s%20by%20example%20yo-limit%20time-ff69b4.svg?style=flat-square)](https://k8.matthewdavis.io)
[![Twitter Follow](https://img.shields.io/twitter/follow/yomateod.svg?label=Follow&style=flat-square)](https://twitter.com/yomateod) [![Skype Contact](https://img.shields.io/badge/skype%20id-appsoa-blue.svg?style=flat-square)](skype:appsoa?chat)

# Kubernetes Redis Cluster

> k8 by example -- straight to the point, simple execution.

## Install

```sh
git clone https://github.com/mateothegreat/k8-byexamples-redis-cluster && cd k8-byexamples-redis-cluster
git submodule update --init
make install
```
# Scale both replication controllers
```sh
kubectl scale rc redis --replicas=3
kubectl scale rc redis-sentinel --replicas=3
```

# See Also
* https://redis.io/topics/cluster-tutorial
* https://github.com/kubernetes/examples/tree/master/staging/storage/redis
