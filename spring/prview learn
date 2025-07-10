
---

### **一、必学核心概念（基础阶段）  
1. **IoC（控制反转）与 DI（依赖注入）**  
   - 理解 `ApplicationContext` 容器的作用  
   - 掌握 XML 配置与注解配置（`@Component`、`@Autowired`）  
   - 手动实现简易 IoC 容器（理解原理）  

2. **Bean 生命周期与管理**  
   - Bean 的作用域：`singleton` vs `prototype`  
   - 生命周期回调：`@PostConstruct`、`@PreDestroy`  
   - FactoryBean 与 BeanPostProcessor 扩展点  

3. **AOP（面向切面编程）**  
   - 掌握动态代理原理（JDK Proxy vs CGLIB）  
   - 使用 `@Aspect` 实现日志、事务等切面  
   - 理解 `Pointcut` 表达式与通知类型（@Before/@Around）  

4. **Spring 数据访问**  
   - JDBC Template 简化数据库操作  
   - 声明式事务管理（`@Transactional` 实现原理）  

---

### **二、渐进式学习路径  
#### **第1阶段：环境搭建与基础配置**  
1. 创建 Maven 项目引入 `spring-core`、`spring-context` 依赖  
2. 通过 XML 配置 Bean（`<bean>` 标签）并启动容器  
3. 迁移到注解配置（`@ComponentScan` + `@Configuration`）  

#### **第2阶段：深度理解 IoC/DI**  
1. 手写简化版 Spring 容器（实现 Bean 加载、依赖注入）  
2. 解决循环依赖问题（三级缓存机制）  
3. 对比 **Setter 注入** vs **构造器注入** 优劣  

#### **第3阶段：AOP 实战**  
1. 用 AOP 实现方法执行时间监控  
2. 通过自定义注解实现权限校验切面  
3. 结合 Spring 事务理解 AOP 代理机制  

#### **第4阶段：整合第三方组件**  
1. 整合 MyBatis（学习 `SqlSessionFactoryBean` 配置）  
2. 集成 RedisTemplate 操作缓存  
3. 配置多数据源与动态数据源切换  

---

### **三、避坑指南与学习技巧  
⚠️ **新人常见误区**：  
- 过度依赖 XML 配置（应先理解后转向注解）  
- 忽视异常类型（`BeanCurrentlyInCreationException` 等需重点理解）  
- 直接使用 Spring Boot 跳过基础（导致原理不清）  

✅ **高效学习方法**：  
1. **调试源码**：从 `ClassPathXmlApplicationContext` 的 `refresh()` 方法入手  
2. **官方文档精读**：重点关注 Core、AOP、Data Access 章节  
3. **画流程图**：Bean 创建流程、AOP 代理过程  
4. **实践驱动**：每学一个概念立即编码验证（例如：修改 Bean 作用域观察现象）  

---

### **四、学习资源推荐  
📚 **文档与书籍**：  
- 官方文档：[Spring Framework Documentation](https://docs.spring.io/spring-framework/reference/)（重点看 Core、AOP）  
- 《Spring 实战（第6版）》：第1-4章精读  
- 《Spring 源码深度解析》：结合源码理解设计思想  

💻 **实战项目**：  
1. 基于 XML/注解配置的超市管理系统（含事务控制）  
2. 使用 AOP 实现 API 调用日志审计系统  
3. 动态数据源切换实现多租户架构  

---

### **五、能力进阶路线  
1. 研究 Spring 设计模式：工厂模式（BeanFactory）、代理模式（AOP）、模板方法（JdbcTemplate）  
2. 分析常见源码：`DefaultSingletonBeanRegistry`、`AbstractAutowireCapableBeanFactory`  
3. 延伸学习：Spring MVC 请求处理流程（为后续 Web 开发打基础）  

建议每天投入 2 小时，配合代码实践，3 个月可掌握 Spring Framework 核心开发能力。遇到问题优先查阅源码注释，其次参考 Spring 官方 Issue 讨论。