To invoke test service throughout the gateway trigger http://ipaddr:8082/eclient/main/test
where
- ipaddr is adress where gateway service is started
- 8082 is a port determined for gateway application in properties file
- eclient is a name of service registered on eureka as client service
- main is an url path to test service functionality determined in @RequestMapping
- test is an url path to test service functionality determined in @GetMapping

It works like that when there are no aliases or additional main url path configured in functional service

To invoke shortened URL path reference to value determined in spring.cloud.gateway.routes[x].predicates[0] properti of gateway application