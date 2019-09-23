# Spring-MVC-study

## Learning DispatcherServlet initialization & service process

##### Spring Version: 4.3.3
##### Build tool: Gradle

#### [스프링 MVC Reference 번역 정보](documents/spring-framework-reference/ko/spring-mvc-translated-version.md)

#### Study Curriculum

##### DispatcherServlet 의 초기화 과정

###### Servlet 의 초기화

###### DispatcherServlet 의 상속구조
- ApplicationContext 구성 및 초기화
    - ApplicationContext 생성: FrameworkServlet#createWebApplicationContext()
    - BeanFactory 생성: AbstractRefreshableApplicationContext#refreshBeanFactory()
    - BeanDefinition 로딩: AnnotationConfigWebApplicationContext:loadBeanDefinitions()
    - BeanPostProcessor 등록: PostProcessorRegistrationDelegate:registerBeanPostProcessors()
    - SingletonBean (전처리)미리 등록: DefaultListableBeanFactory:preInstantiateSingletons()
    
##### 웹 요청의 처리 과정

###### 
