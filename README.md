# spicedb-postgres-kubernetes
Setting spicedb with postgresql db in kind kubernetes

* [Kubernetes-kind](./kind-kube-setup/README.md)
* [Postgres](./postgres/README.md)
* [Spicedb](./spicedb/README.md)


grpcurl -plaintext spicedb-grpc.127.0.0.1.nip.io:80 list
# authzed.api.v1.ExperimentalService
# authzed.api.v1.PermissionsService
# authzed.api.v1.SchemaService
# authzed.api.v1.WatchService
# grpc.health.v1.Health
# grpc.reflection.v1alpha.ServerReflection

# Zed client

zed schema write spicedb-schema.zed --endpoint spicedb-grpc.127.0.0.1.nip.io:80 --insecure --token "foobar"