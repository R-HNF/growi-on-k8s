# growi-on-k8s

GKE(Google Kubernetes Engine)での利用を想定しています。

名前空間は`growi-on-k8s`としています。

以下のイメージは[weseek/growi-docker-compose](https://github.com/weseek/growi-docker-compose)のDockerfileからビルドしています。
- `gcr.io/example-project-id/-growi-on-k8s-growi`
- `gcr.io/example-project-id/growi-on-k8s-es`

## 構成
Growi, Elasticsearch, MongoDBには`Statefulset`を利用しています。

外部公開には`Ingress`を利用しています。

IPアクセス制限のためにGCPのCloud Armorを利用しています。