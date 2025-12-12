# Backend Lab

这是一个基于 Docker Compose 构建的模块化后端中间件练习环境，旨在方便地管理 Redis、MySQL、Kafka 等服务。项目结构将每个服务的数据（Data）和配置隔离在各自的子目录下（如 `./redis/data`），确保环境整洁且数据在容器重启后依然持久化保存。

使用时，你可以灵活地按需启动特定服务，例如运行 `docker-compose up -d redis` 仅启动 Redis。Redis 服务已默认映射至宿主机 `6379` 端口，密码预设为 `123456`，你可以通过 `docker exec -it lab-redis redis-cli` 进入容器内部练习，或直接使用图形化工具连接。