消息处理与Action类的mapping对应(使用注解类的方式)

一般来说Action中应该有自己的实际业务处理类,那么上述方式可能不妥

推荐用org.springframework.context.ApplicationContext#getBeansWithAnnotation函数

当然,也可以重写AbstractActionMapping类实现自己的Mapping