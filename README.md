#REST

##@RestController
-class level annotation used for the resource class. It is a combination of
@Controller and @ResponseBody and because of it, class returns a domain
object instead of a view.

##@RequestMapping
-is used at class level to map the /calculation URI to CalculationController
class. It ensures the HTTP request to /calculation is mapped to the CalculationController class.
Based on the path defined using the annotation @RequestMapping of the URI it would be mapped to respective 
methods. 

##@RequestParam
-is responsible for binding the query parameter to the parameter of the controllers method.
For example, the QueryParam base and exponent are bound to parameters b and e of method pow of 
CalculationController respectively. Both of the query parameters of the  pow() method are 
required as we're not using and default values.

e.g @RequestParam(value="base", defaultValue="2") 

here if the user does not pass a value the default will be used.

##@PathVariable
-helps you create the dynamic URIs and allows you to map Java parameters to a path parameter. 
It works with @RequestMapping where placeholder is created in URI then the same placeholder
name is used either as a PathVariable or a method parameter.

##@SpringBootApplication

##@Configuration
-tags the class as a source of Bean definitions for the application context.

##@EnableAutoConfiguration
-indicates that SpringBoot is to start adding beans based on classpath settings, other beans and
various property settings.

##@EnableWebMvc
-is added if Spring Boot finds the spring-webmvc on the classpath. It treats the application as a web 
application and activates key behaviours such as setting up a DispatcherServlet.

##@ComponentScan
-tells Spring to look for other components, configurations and services in the given package.