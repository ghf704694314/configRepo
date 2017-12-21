# configRepo
As a springCloud-config repo for demo




###zuul分析需要用到的类

com.netflix.zuul(netflix公司)
IZuulFilter 接口,定义shouldFilter和run方法
ZuulFilter filter抽象父类 实现IZuulFilter并给子类规定了filterType和filterOrder方法实现
ZuulFilterResult 封装了filter执行结果
ZuulRunner 调用FilterProcessor执行filter
FilterProcessor 真正执行filter.run方法的类
ZuulServlet 调用ZuulRunner执行FilterProcessor
RequestContext zuul请求上下文
ZuulConstants zuul常量
FilterFileManager 轮询filter文件目录
FilterLoader filter加载器


org.springframework.cloud.netflix.zuul(结合springCloud)

FilterConstants filter常量
ZuulProperties zuul常量
以及zuul.filters下的preFilters,routeFilters,postFilters,errorFilter