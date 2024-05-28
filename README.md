# 一杯云外卖（苍穹外卖学习）
## 一、项目配置
### 1. 前端代码启动
前端基于Nginx启动

### 2. redis服务端启动
redis-server.exe redis.windows.conf

### 3. 后端代码启动
- 1. 在配置application-dev中配置mysql数据库信息
- 2. 配置阿里云对象存储OSS信息
- 3. 配置redis数据信息
- 4. 配置wx小程序信息
  
### 4. wx小程序启动


## 二、项目技术（后端）
### 1. Swagger：生成接口文档，进行后端接口测试
### 2. PageHelper实现查询分页
### 3. 采用自定义注解AutoFill、自定义切面类AutoFillAspect实现填充公共字段
### 4. 编写redis配置类，创建redis模板类RedisTemplate对象，来操作redis
### 5. 采用Spring Cache实现菜品、套餐数据缓存功能，@EnableCaching（开启缓存注解功能）、@Cacheable（有则返回，无则放入数据）、@CachePut（返回值放入）、@CacheEvict（删除）
### 6. Spring Task：采用@Scheduled(cron = "0 * * * * ? ") 注解进行定时任务
### 7. 导入WebSocket服务组件WebSocketServer，导入配置类WebSocketConfiguration，注册WebSocket服务组件