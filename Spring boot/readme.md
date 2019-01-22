## 搭建一个Spring boot 项目
第一种方法http://start.spring.io/压缩包

@RestController相当于@Controller + @ResponseBody
@Component 

spring-boot-starter其中包含了 spring-boot-starter-logging，该依赖内容就是 Spring Boot 默认的日志框架 logback。  
默认情况下，Spring Boot将日志输出到控制台，不会写到日志文件。如果要编写除控制台输出之外的日志文件，则需在application.properties中设置logging.file或logging.path属性。 <br>
logging.file，设置文件，可以是绝对路径，也可以是相对路径。如：logging.file=my.log  
logging.path，设置目录，会在该目录下创建spring.log文件，并写入日志内容，如：logging.path=/var/log  
> 如果只配置 logging.file，会在项目的当前路径下生成一个 xxx.log 日志文件。 <br> 
如果只配置 logging.path，在 /var/log文件夹生成一个日志文件为 spring.log  
注：二者不能同时使用，如若同时使用，则只有logging.file生效





参考链接:https://www.cnblogs.com/ityouknow/p/5662753.html

疑问:时钟序列、序列化与反序列化
@BatchSize

uuid
@GeneratedValue(generator = "generator")
@GenericGenerator(name = "generator", strategy = "uuid2")
