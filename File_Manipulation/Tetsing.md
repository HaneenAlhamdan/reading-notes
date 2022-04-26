### Testing and Swagger and Deployment


## Swagger 

is a powerful yet easy-to-use suite of API developer tools for teams and individuals, enabling development across the entire API lifecycle, from design and documentation, to test and deployment.


## The OpenAPI

 is the official name of the specification. The development of the specification is fostered by the OpenAPI Initiative, which involves more the 30 organizations from different areas of the tech world — including Microsoft, Google, IBM, and CapitalOne. Smartbear Software, which is the company that leads the development of the Swagger tools, is also a member of the OpenAPI Initiative, helping lead the evolution of the specification.

 ![ApiInfor](https://user-images.githubusercontent.com/98957434/165206108-3d709b46-f6fb-4636-84af-0941f4a6fb33.png)



![qT9N8](https://user-images.githubusercontent.com/98957434/165205326-dc08866b-c919-4119-950d-7166fc9ecf4d.png)

## Unit test

In the software development process Unit Tests basically test individual parts ( also called as Unit ) of code (mostly methods) and make it work as expected by programmer. A Unit Test is a code written by any programmer which test small pieces of functionality of big programs. Performing unit tests is always designed to be simple, A "UNIT" in this sense is the smallest component of the large code part that makes sense to test, mainly a method out of many methods of some class. Generally the tests cases are written in the form of functions that will evaluate and determine whether a returned value after performing Unit Test is equals to the value you were expecting when you wrote the function. The main objective in unit testing is to isolate a unit part of code and validate its to correctness and reliable. 


namespace nH.MasterData.API.Controllers
{
    [Produces("application/json")]
    [Route("api/AType")]
    public class ATypeController : Controller
    {
        private readonly IProcessor _domain;
        private readonly ILogger _logger;
        private const string Version = "VERSION_1";
        private const string Model = "model";
        private const string Entity = "AType";

        public ATypeController(IProxy proxy, ILogger<ATypeController> logger)
        {
            _logger = logger;
            var proxy = proxy.GetProxy();
            _domain = new InstitutionAddressProcessor(proxy);
        }

        [HttpGet]
        public OkObjectResult Get()
        {
            try
            {
                return Ok(_domain.GetATypesMembers(Model, Version, Entity, MemberType.Leaf, null));
            }
            catch (Exception ex)
            {
                _logger.LogError(ex.Message + " " + ex.StackTrace);
                return new OkObjectResult(BadRequest());
            }
        }

    }
}