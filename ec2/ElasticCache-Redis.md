
进入redis

redis-cli -h 127.0.0.1 -p 6379

备份

RDB: redis-cli -h 127.0.0.1 -p 6379 -a pwd bgsave

AOF: redis-cli -h 127.0.0.1 -p 6379 -a pwd bgrewriteaof

获得 appendonly.aof, dump.rbd 文件，随后将该文件放入到redis的安装路径下



获取安装路径

CONFIG GET dir

重启redis即可恢复



	
vylyv-api-redis-001.iqdxbs.0001.usw2.cache.amazonaws.com

## 亚马逊云redis，先备份后再使用复制功能将rdb文件放入到S3桶存储
