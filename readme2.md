### 源码阅读
* 源码阅读的原则
  * 带着问题阅读
  
  * 看不懂或无关细节跳过

  * 跑不起来不读
  
    
  
* 问题列表``
  * Bean的整体生命周期
  * spring如何解决循环依赖？spring如何解决循环依赖？如果只保留二级缓存行不行？
  * 
* 
  
* 测试用例
  * spring-context
  
    ```java
     1. 解析 XML 配置文件成对应的 BeanDefinition 们的流程
      * org.springframework.beans.factory.xml.XmlBeanDefinitionReaderTests#withFreshInputStream()
    
     2. 加载 Bean 的流程
      * org.springframework.beans.factory.xml.AbstractBeanFactoryTests
      
     3. ClassPathXmlApplicationContext的流程
      * org.springframework.context.support.ClassPathXmlApplicationContextTests#testResourceAndInputStream()
      
    ```
  
  * spring-tx
  
    ```
     1. 调试 <tx:advice /> 标签的解析的流程
      * org.springframework.transaction.TxNamespaceHandlerTests
         #invokeTransactional() 方法，提交事务。
         #rollbackRules() 方法，回滚事务。
     2. 调试 @Transactional 注解的解析的流程
      * org.springframework.transaction.TxNamespaceHandlerTests 
    ```
  
    
  
  * ss
  
  * sss
  
  * s
  
  * ss
  
  *  
  
  

