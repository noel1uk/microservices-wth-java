REST

@RestController
-class level annotation used for the resource class. It is a combination of
@Controller and @ResponseBody and because of it, class returns a domain
object instead of a view.

@RequestMapping
-is used at class level to map the /calculation URI to CalculationController
class