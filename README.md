# Couchbase Docker Image For Testcontainers

This project is provides pre initialized Couchbase over docker with environment variables for testcontainers.

You can pull over docker hub;
```sh
docker pull docker.io/trendyoltech/couchbase-testcontainer
```

Configurable environment variables are following;


```sh
ENV SERVICES "data,index,query,fts,analytics,eventing"

ENV CLUSTER_RAMSIZE 1024
ENV CLUSTER_INDEX_RAMSIZE 512
ENV CLUSTER_EVENTING_RAMSIZE 256
ENV CLUSTER_FTS_RAMSIZE 256
ENV CLUSTER_ANALYTICS_RAMSIZE 1024

ENV INDEX_STORAGE_SETTING "memopt"

ENV BUCKET_NAME "Sample"
ENV BUCKET_TYPE "couchbase"
ENV BUCKET_RAMSIZE 128

ENV USERNAME "Administrator"
ENV PASSWORD "password"

ENV REST_PORT 8091
ENV CAPI_PORT 8092
ENV QUERY_PORT 8093
ENV FTS_PORT 8094
ENV MEMCACHED_SSL_PORT 11207
ENV MEMCACHED_PORT 11210
ENV SSL_REST_PORT 18091
```

See following links for detailed usage;
- [Automated Integration Testing over Gitlab CI/CD for Dotnet Core via Testcontainers](https://medium.com/trendyol-tech/automated-integration-testing-over-gitlab-ci-cd-for-dotnet-core-via-testcontainers-b18c7f81e65f)
- [Couchbase Integration Testing For Golang Via Testcontainers](https://medium.com/trendyol-tech/couchbase-integration-testing-for-golang-via-testcontainers-25b906bc2c0d)
