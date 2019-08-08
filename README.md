# 环境列表
- redis 5.0.5 
- docker-compose

# 开启 
`docker-compose up -d`

# 集群快速搭建
```
redis-cli --cluster create 127.0.0.1:7000 127.0.0.1:7001 \
127.0.0.1:7002 127.0.0.1:7003 127.0.0.1:7004 127.0.0.1:7005 \
--cluster-replicas 1 
```

# 细节
如果想了解细节如握手、主从等可以参考[docker-compose搭建redis集群及可用性实践](https://juejin.im/post/5d4afaaf518825403769dd44)