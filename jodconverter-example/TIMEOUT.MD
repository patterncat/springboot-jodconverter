2017-10-22 15:45:08.938  INFO 4408 --- [nio-8080-exec-1] c.p.e.controller.ConvertController       : output file :/var/folders/9r/v55wkcr91m5_g8h7lhgjzgr00000gn/T/tmp4117106826520524919.pdf
2017-10-22 15:45:08.948  INFO 4408 --- [   task-queue-2] o.jodconverter.task.LocalConversionTask  : Executing local conversion task...
2017-10-22 15:45:11.978 ERROR 4408 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/].[dispatcherServlet]    : Servlet.service() for servlet [dispatcherServlet] in context with path [] threw exception [Request processing failed; nested exception is org.jodconverter.office.OfficeException: task execute timeout] with root cause

java.util.concurrent.TimeoutException: null
	at java.util.concurrent.FutureTask.get(FutureTask.java:205) ~[na:1.8.0_71]
	at org.jodconverter.office.OfficeManagerAdapter.execute(OfficeManagerAdapter.java:69) ~[classes/:4.1.0]
	at org.jodconverter.LocalConverter$LocalConversionJob.doExecute(LocalConverter.java:174) ~[jodconverter-local-4.1.0.jar:4.1.0]
	at org.jodconverter.job.AbstractConversionJob.execute(AbstractConversionJob.java:57) ~[jodconverter-core-4.1.0.jar:4.1.0]
	at cn.patterncat.example.controller.ConvertController.convert(ConvertController.java:49) ~[classes/:na]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[na:1.8.0_71]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[na:1.8.0_71]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[na:1.8.0_71]
	at java.lang.reflect.Method.invoke(Method.java:497) ~[na:1.8.0_71]
	at org.springframework.web.method.support.InvocableHandlerMethod.doInvoke(InvocableHandlerMethod.java:205) ~[spring-web-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.method.support.InvocableHandlerMethod.invokeForRequest(InvocableHandlerMethod.java:133) ~[spring-web-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.servlet.mvc.method.annotation.ServletInvocableHandlerMethod.invokeAndHandle(ServletInvocableHandlerMethod.java:97) ~[spring-webmvc-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerAdapter.invokeHandlerMethod(RequestMappingHandlerAdapter.java:827) ~[spring-webmvc-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerAdapter.handleInternal(RequestMappingHandlerAdapter.java:738) ~[spring-webmvc-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.servlet.mvc.method.AbstractHandlerMethodAdapter.handle(AbstractHandlerMethodAdapter.java:85) ~[spring-webmvc-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.servlet.DispatcherServlet.doDispatch(DispatcherServlet.java:967) ~[spring-webmvc-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.servlet.DispatcherServlet.doService(DispatcherServlet.java:901) ~[spring-webmvc-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.servlet.FrameworkServlet.processRequest(FrameworkServlet.java:970) ~[spring-webmvc-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.servlet.FrameworkServlet.doPost(FrameworkServlet.java:872) ~[spring-webmvc-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at javax.servlet.http.HttpServlet.service(HttpServlet.java:661) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.springframework.web.servlet.FrameworkServlet.service(FrameworkServlet.java:846) ~[spring-webmvc-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at javax.servlet.http.HttpServlet.service(HttpServlet.java:742) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.ApplicationFilterChain.internalDoFilter(ApplicationFilterChain.java:231) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.ApplicationFilterChain.doFilter(ApplicationFilterChain.java:166) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.tomcat.websocket.server.WsFilter.doFilter(WsFilter.java:52) ~[tomcat-embed-websocket-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.ApplicationFilterChain.internalDoFilter(ApplicationFilterChain.java:193) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.ApplicationFilterChain.doFilter(ApplicationFilterChain.java:166) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.springframework.web.filter.RequestContextFilter.doFilterInternal(RequestContextFilter.java:99) ~[spring-web-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.filter.OncePerRequestFilter.doFilter(OncePerRequestFilter.java:107) ~[spring-web-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.apache.catalina.core.ApplicationFilterChain.internalDoFilter(ApplicationFilterChain.java:193) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.ApplicationFilterChain.doFilter(ApplicationFilterChain.java:166) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.springframework.web.filter.HttpPutFormContentFilter.doFilterInternal(HttpPutFormContentFilter.java:105) ~[spring-web-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.filter.OncePerRequestFilter.doFilter(OncePerRequestFilter.java:107) ~[spring-web-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.apache.catalina.core.ApplicationFilterChain.internalDoFilter(ApplicationFilterChain.java:193) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.ApplicationFilterChain.doFilter(ApplicationFilterChain.java:166) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.springframework.web.filter.HiddenHttpMethodFilter.doFilterInternal(HiddenHttpMethodFilter.java:81) ~[spring-web-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.filter.OncePerRequestFilter.doFilter(OncePerRequestFilter.java:107) ~[spring-web-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.apache.catalina.core.ApplicationFilterChain.internalDoFilter(ApplicationFilterChain.java:193) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.ApplicationFilterChain.doFilter(ApplicationFilterChain.java:166) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.springframework.web.filter.CharacterEncodingFilter.doFilterInternal(CharacterEncodingFilter.java:197) ~[spring-web-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.springframework.web.filter.OncePerRequestFilter.doFilter(OncePerRequestFilter.java:107) ~[spring-web-4.3.9.RELEASE.jar:4.3.9.RELEASE]
	at org.apache.catalina.core.ApplicationFilterChain.internalDoFilter(ApplicationFilterChain.java:193) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.ApplicationFilterChain.doFilter(ApplicationFilterChain.java:166) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.StandardWrapperValve.invoke(StandardWrapperValve.java:198) ~[tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.StandardContextValve.invoke(StandardContextValve.java:96) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.authenticator.AuthenticatorBase.invoke(AuthenticatorBase.java:478) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.StandardHostValve.invoke(StandardHostValve.java:140) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.valves.ErrorReportValve.invoke(ErrorReportValve.java:80) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.core.StandardEngineValve.invoke(StandardEngineValve.java:87) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.catalina.connector.CoyoteAdapter.service(CoyoteAdapter.java:342) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.coyote.http11.Http11Processor.service(Http11Processor.java:799) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.coyote.AbstractProcessorLight.process(AbstractProcessorLight.java:66) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.coyote.AbstractProtocol$ConnectionHandler.process(AbstractProtocol.java:861) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.tomcat.util.net.NioEndpoint$SocketProcessor.doRun(NioEndpoint.java:1455) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at org.apache.tomcat.util.net.SocketProcessorBase.run(SocketProcessorBase.java:49) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1142) [na:1.8.0_71]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:617) [na:1.8.0_71]
	at org.apache.tomcat.util.threads.TaskThread$WrappingRunnable.run(TaskThread.java:61) [tomcat-embed-core-8.5.15.jar:8.5.15]
	at java.lang.Thread.run(Thread.java:745) [na:1.8.0_71]

2017-10-22 15:45:17.659  INFO 4408 --- [   task-queue-2] o.j.office.OfficeManagerAdapter          : finish task execution
