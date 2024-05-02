# xtquantservice
基于讯投miniqmt封装的服务API服务。
特别适合量化系统较复杂系统，如多证券账户的场景，微服务架构的量化交易系统。 
常用功能有： 持仓查询、资金查询、委托订单、成交订单查询等功能。 
支持执行回调，以便于日志生成、微信消息提醒等功能实现。 

# 技术架构
- 基于讯投miniqmt封装的xtquant，功能强大，使用简单。
- 基于当前最优秀的python后端框架fastapi实现，性能杠杠的。 
- 基于loguru，日志记录简单方便。
- 基于uvicorn，服务启动简单方便。

# 目录介绍
- xtquant : 来自官网的xtquant sdk，当前使用版本 xtquant_240329
- demo  ： 示例代码，基于xtquant_240329实现
- tests ： 单元测试
- xtquantservice ： 项目核心代码，一个基于xtquant封装的服务API服务，基于fastapi实现。
- xtquantservice.main ： 项目入口，基于uvicorn启动服务。
- xtquantservice.settings ： 项目配置文件。

# 快速开始

## 1. 安装依赖

```
pip install -r requirements.txt
```

## 2. 启动服务

```
uvicorn xtquantservice.main:app --host 0.0.0.0 --port 8000
```



# 备注

还没开发完，急需可以私信我。