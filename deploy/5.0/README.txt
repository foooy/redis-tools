redis-5.X.Y版本的配置文件模板

如果开启了aof，建议save参数调大一点，减少写rdb文件频率，比如可以考虑如下配置：
save 900 10
save 300 100
save 60 100000
相比默认配置提高了10倍。
