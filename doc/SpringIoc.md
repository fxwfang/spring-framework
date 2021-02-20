### Spring IOC

```
问题：
1. Spring IOC 流程图
2. 在Spring的整个创建过程中，如果想在不同的阶段做不同的事情要怎么处理？
3. Spring循环依赖三级缓存是否可以减少为二级缓存？
4. 三级缓存为什么要包装一层ObjectFactory对象？
```

### 测试类
ClassPathXmlApplicationContextTests.testSingleConfigLocation


### Spring IOC流程图

![image-20210206002209312](/Users/fangxiaowei/IdeaProjects/spring-framework/doc/images/image-20210206002209312.png)

```
大致流程： BeanFactory -- > BeanDefinition --> beanFactoryProcessor --> 实例化 --> 填充属性 --> BeanPosyProcessorBefore -->....


```



### Spring 循环依赖问题

![image-20210206224115767](/Users/fangxiaowei/IdeaProjects/spring-framework/doc/images/image-20210206224115767.png)‘’‘

>https://www.processon.com/view/5d2d7e14e4b0511f1306ce3b?fromnew=1







### 在Spring的整个创建过程中，如果想在不同的阶段做不同的事情要怎么处理？

观察者模式：监听器(事件发布)



### BeanFactory & FactoryBean

* BeanFactory 需要走完完整的初始化流程才能使用

* FactoryBean  定制化的实例化bean

  ```
  BeanFactory是个Factory，也就是IOC容器或对象工厂，FactoryBean是个Bean。
  ```

  



