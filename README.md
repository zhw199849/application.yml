spring:
  profiles:
    active:
    - dev
---
server:
  port: 8003
spring:
  application:
    name: USER-PROVIDER  #服务的名字
  profiles: dev
eureka:
  client:
    service-url:
      defaultZone: http://localhost:7001/eureka  #服务注册的注册中心的地址


---
server:
  port: 8004
spring:
  application:
    name: USER-PROVIDER  #服务的名字
  profiles: test
eureka:
  client:
    service-url:
      defaultZone: http://localhost:7001/eureka  #服务注册的注册中心的地址
