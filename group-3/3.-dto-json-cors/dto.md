# DTO

정의&#x20;

Data Transfer Object



1. 아주 단순하게 보면 setter와 getter로만 이뤄짐.
2. JavaBeans에서 유래한 Java Bean 또는 그냥 Bean이라고 부르는 형태에 가까움(Spring Bean, POJO와 다름에 주의..).
   * [JavaBeans](https://ko.wikipedia.org/wiki/%EC%9E%90%EB%B0%94%EB%B9%88%EC%A6%88)
   * [Introduction to the Spring IoC Container and Beans](https://docs.spring.io/spring-framework/docs/6.0.x/reference/html/core.html#beans-introduction)
3. 제대로 된 객체가 아니라 그냥 무기력한 데이터 덩어리. C/C++ 등에선 구조체(struct)로 구분할 수 있지만, Java에선 불가능. 최신 Java에선 record를 활용할 수 있지만, 오래된 Bean 관련 라이브러리에선 지원하지 않음.





### Tier간의 통신

* F/E 와 B/E 사이 에서 사용
* DTO 자체를 그대로 전송할 수 없다. 그래서 직렬화(마샬링)을 한다.
* 그래서 어떤 직렬화 기술을 사용할 건지 결정해야함 -> JSON, XML(JSON이 단순하고 사용하기 쉬기 때문에 제이슨을 사용)
* BE 와 BD 사이 -> 여기 사이에서도 DTO사용



