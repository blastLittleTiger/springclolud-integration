服务降级的说明

使用了springcloud-api-feign-hystrix提供的接口service-api
降级功能配合了feign，虽然服务端`provider`引用了这个接口，但是服务的降级，是在`consumer`上面控制的。
相关的工程有`springcloud-api-feign-hystrix`这个是api,`springcloud-consumer-feign-hystrix-8901`这个是consumer, 
`springcloud-provider-demote-8004`这个是provider。