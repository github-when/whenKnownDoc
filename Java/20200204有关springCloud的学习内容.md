集团客户项目组协助文件

地址:

​	git@gitee.com:hantao_1997/gitStudy.git



我的账号:whenknow

密码:768445003.jinwen





springcloud五大组件:

​	 1.1.**Eureka service**:注册中心,里面有一个注册表,保存了各个服务所在的机器和端口号

​	 1.2.**Eurake Client**:负责将这个服务的信息注册到Eureka Server中

​	2. Feign:动态代理调用

​	3.**Ribbon**负载均衡

注:**，Ribbon是和Feign以及Eureka紧密协作**

​	4.**Hystrix**隔离、熔断以及降级的一个框架

​	5.Zuul:微服务网关,这个组件是负责网络路由的!

总结:

Eureka:个服务启动时,Eureka会将服务注册到EurekaService,并且EurakeClient还可以返回过来从EurekaService拉去注册表,从而知道服务在哪里

Ribbon:服务间发起请求的时候,基于Ribbon服务做到负载均衡,从一个服务的对台机器中选择一台

Feign:基于fegin的动态代理机制,根据注解和选择机器,拼接Url地址,发起请求

Hystrix:发起的请求是通过Hystrix的线程池来走,不同的服走不同的线程池,实现了不同的服务调度隔离,避免服务雪崩的问题 

Zuul:如果前端后端移动端调用后台系统,统一走zull网关进入,有zull网关转发请求给对应的服务

//逻辑

//1.取出四张表中的所有数据

//2.对每张表的数据进行TreeMap存储[默认升序排列,可自定义比较器]

//3.存储内容,key=20190101 .value= ArrayList    后续数据为同样日期,取出ArrayList,add后,重新放入

//4.对四张表进行排序

//5.最终数据 遍历整合.

​		key   value :ArrayList[0]

​							ArrayList[1]




