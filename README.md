springcloud 学习笔记
------------------------------
#### eurekaserver:服务注册和发现模块
#### service-hi:服务提供者
#### service-ribbon: 负载均衡客户端(Hystrix断路由服务消费者)
###### Ribbon is a client side load balancer which gives you a lot of control over the behaviour of HTTP and TCP clients. Feign already uses Ribbon, so if you are using @FeignClient then this section also applies.—–摘自官网
###### ribbon 是一个负载均衡客户端，可以很好的控制htt和tcp的一些行为。Feign也用到ribbon，当你使用@ FeignClient，ribbon自动被应用。
#### service-feign: 负载均衡客户端 (Hystrix断路由服务消费者)
`Feign是一个声明式的web服务客户端，它使得写web服务变得更简单。使用Feign,只需要创建一个接口并注解。它具有可插拔的注解特性，包括Feign 注解和JAX-RS注解。Feign同时支持可插拔的编码器和解码器。spring cloud对Spring mvc添加了支持，同时在spring web中次用相同的HttpMessageConverter。当我们使用feign的时候，spring cloud 整和了Ribbon和eureka去提供负载均衡。`
#### Hystrix:断路由
` http://localhost:port/hystrix 仪表盘地址`

#### service-zuul: 路由网关
Zuul的主要功能是路由和过滤器。路由功能是微服务的一部分，比如／api/user映射到user服务，/api/shop映射到shop服务。zuul实现了负载均衡。

##### zuul有以下功能：
- Authentication
- Insights
- Stress Testing
- Canary Testing
- Dynamic Routing
- Service Migration
- Load Shedding
- Security
- Static Response handling
- Active/Active traffic management

