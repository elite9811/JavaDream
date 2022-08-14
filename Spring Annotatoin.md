## **Core Spring Framework Annotation**

>***@Required*** : 
> + apply to the bean setter method. 
> + It indicates that the annotated bean must be populated at configuration time with the required property, else it throws an exception **BeanInitilizationException**

>***@Autowired***
> + provides annotation-based auto-wiring 
> + It is used to autowire spring bean on setter methods, instance variable, and constructor. When we use ***@Autowired*** annotation, the spring container auto-wires the bean by matching data-type.

>***@Configuration***
> + *class-level* 
> + The class annotated with ***@Configuration*** used by Spring Containers as a source of bean definitions.

>***@Bean*** 
> + *method-level* 
> + alternative of XML \<bean> tag
> + It tells the method to produce a bean to be managed by Spring Container.

## **Spring Framework Stereotype Annotations**

>***@Component***
> + *class-level* 
> + It is used to mark a Java class as a bean. A Java class annotated with ***@Component*** is found during the classpath. The Spring Framework pick it up and configure it in the application context as a **Spring Bean**.

>***@Controller*** 
> + *class-level*
> + It is a specialization of ***@Component***. It marks a class as a web request handler. It is often used to serve web pages. By default, it returns a string that indicates which route to redirect. It is mostly used with ***@RequestMapping*** annotation

>***@Service***
> + *class level*. 
> + It tells the Spring that class contains the business logic.

>***@Repository***
> + *class-level* 
> + The repository is a **DAO**s (Data Access Object) that access the database directly. The repository does all the operations related to the database.

## **Spring Boot Annotations**
>***@EnableAutoConfiguration***
> + It auto-configures the bean that is present in the classpath and configures it to run the methods. 
> + The use of this annotation is reduced in Spring Boot 1.2.0 release because developers provided an alternative of the annotation, i.e. ***@SpringBootApplication***.

>***@SpringBootApplication***
> + It is a combination of three annotations 
>> + @EnableAutoConfiguration
>> + @ComponentScan 
>> + @Configuration.

## **Spring MVC and REST Annotations**

> If you want to see, click [here](https://www.javatpoint.com/spring-boot-annotations)

## Extra

### Each entity must have at least 2 annotations defined: *@Entity* and *@Id*.

>***@Entity***
> + specify that the class is an entity
> + is mapped to a database table

>***@Table***
> + specify the name of the database table to be used for mapping

>***@Id***
> + specify the primary key of an entity

>***@GeneratedValue***
> + provide for the specification of generation strategies for the values of primary keys

>***@Override***
> + default Java annotation
> + introduced in Java 1.5
> + indicate that the child class method is overwriting its base class method
> + extract a warning from the compiler if the annotated method doesn't actually override anything
> + benefits
>> - take advantage of the compiler checking to make sure you actually are overriding a method when you think you are
>> - make your code easier to understand 'cause it is more obvious when methods are overwritten

> ***@JsonIgnoreProperties***
> + `from the Jackson JSON processing library`
> + `indicate that any properties not bound in this type should be ignored`
> + `In CASE your variable name and key in JSON doc don't match, you can use @JsonProperty annotation to specify the exact key of the JSON document`

