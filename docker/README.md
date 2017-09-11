```
docker-compose up -d
docker-compose exec etcd etcd --version
docker-compose exec etcd /bin/sh -c "ETCDCTL_API=3 /usr/local/bin/etcdctl version"
docker-compose exec etcd /bin/sh -c "ETCDCTL_API=3 /usr/local/bin/etcdctl endpoint health"
docker-compose exec etcd /bin/sh -c "ETCDCTL_API=3 /usr/local/bin/etcdctl put foo bar"
docker-compose exec etcd /bin/sh -c "ETCDCTL_API=3 /usr/local/bin/etcdctl get foo"
```
