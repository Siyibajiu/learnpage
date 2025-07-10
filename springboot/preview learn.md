
---

### **一、基础核心内容**
1. **Spring Boot 入门**
   - **环境搭建**：JDK、Maven/Gradle、IDE（推荐 IntelliJ IDEA）
   - **项目创建**：使用 [Spring Initializr](https://start.spring.io/) 快速生成项目骨架。
   - **核心机制**：理解 `@SpringBootApplication` 注解、自动配置（Auto-Configuration）、起步依赖（Starter Dependencies）。

2. **Web 开发基础**
   - **RESTful API 开发**：`@RestController`、`@RequestMapping`、`@GetMapping` 等注解。
   - **HTTP 请求处理**：参数接收（`@RequestParam`、`@PathVariable`）、JSON 序列化（Jackson）。
   - **静态资源处理**：默认路径配置（`/static`, `/public`）。

3. **数据访问**
   - **Spring Data JPA**：掌握 `JpaRepository`、实体类注解（`@Entity`、`@Table`）、关联关系（`@OneToMany`）。
   - **整合 MyBatis**：`@Mapper` 接口、XML 映射文件。
   - **数据库配置**：`application.properties` 中配置数据源（DataSource）、连接池（HikariCP）。

4. **配置文件**
   - 多环境配置：`application-dev.yml`、`application-prod.yml`。
   - 配置优先级：命令行参数 > 系统变量 > 配置文件。

---

### **二、进阶技能**
1. **AOP 与事务管理**
   - **AOP 切面编程**：日志、权限校验等场景（`@Aspect`、`@Around`）。
   - **事务控制**：`@Transactional` 注解与传播行为（Propagation）。

2. **安全与鉴权**
   - **Spring Security**：用户认证（Authentication）、权限控制（`@PreAuthorize`）、JWT 集成。

3. **缓存与性能优化**
   - **Spring Cache**：`@Cacheable`、`@CacheEvict`，整合 Redis 缓存。
   - **异步处理**：`@Async` 异步方法、线程池配置。

4. **接口文档与测试**
   - **Swagger/OpenAPI**：自动生成 API 文档（`@Operation`、`@ApiResponse`）。
   - **单元测试**：`@SpringBootTest`、MockMvc 模拟 HTTP 请求。

5. **异常处理**
   - 全局异常处理：`@ControllerAdvice` + `@ExceptionHandler`。
   - 自定义异常类与统一响应封装。

---

### **三、扩展与实战**
1. **微服务与 Spring Cloud**
   - 服务注册与发现：Eureka/Nacos。
   - 服务调用：OpenFeign、负载均衡（Ribbon）。
   - 配置中心：Spring Cloud Config。

2. **消息队列**
   - 整合 RabbitMQ/Kafka：消息生产与消费（`@RabbitListener`）。

3. **部署与监控**
   - 打包与运行：生成可执行 JAR，多环境部署。
   - **Docker 化部署**：编写 Dockerfile、容器化运行。
   - **监控**：Spring Boot Actuator、Prometheus + Grafana。

4. **性能调优**
   - JVM 参数优化（堆内存、GC 策略）。
   - SQL 慢查询分析与索引优化。

---

### **四、学习资源推荐**
- **官方文档**：[Spring Boot Reference](https://spring.io/projects/spring-boot)（必读！）
- **书籍**：《Spring Boot实战》《Spring微服务实战》
- **实战项目**：电商后台、博客系统、OA系统（GitHub 搜索关键词：`springboot-shop`、`springboot-blog`）
- **社区**：Stack Overflow、Spring 中文网。

---

### **避坑指南**
- ❌ 不要跳过 Spring Framework 直接学 Spring Boot（理解 IoC、DI 是关键）。
- ❌ 避免过度依赖自动配置：了解原理（查看 `spring-boot-autoconfigure` 源码）。
- ✅ 多用 Debug 和日志：深入理解请求处理流程和 Bean 生命周期。

按照这个路线逐步实践，边学边写代码，2-3 个月即可熟练掌握 Spring Boot 开发！遇到问题优先查阅官方文档和源码注释，这是最权威的学习方式。