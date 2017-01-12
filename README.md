﻿#zeus-php

## 图例
![alt 架构][id]

[id]: https://github.com/nathena/zeus-php/blob/master/resource/1.jpg "架构"

## 写在前面的话
为什么创建了zeus-php这个项目，并逐步衍生成一个框架（小型？）？其原因其实是一直以来在考虑，如何将clean或ddd架构使用于php项目中（接触过很多项目，新的或旧的，很多组员都考虑如何设计数据库。）。
实际上个人觉得，良好的架构一并不是数据库优先，而是业务模型优先。架构一个系统，优先确定业务模型间的关系，基于内存实现业务逻辑，异步持久化到硬盘（数据库）。这样的架构，在扩展或性能上可以找到很好的临界值。
因此，处于这些考虑慢慢着手写了zeus-php的代码。

## 文档
### etc
- config.php： 默认项目环境配置文件，项目可根据实际情况使用APP_ENV_DIR常量重载。关于APP_ENV_DIR，详见[zeus\foundation\ConfigManager](#ConfigManager)


### zeus\foundation\ConfigManager<a name="ConfigManager" />
