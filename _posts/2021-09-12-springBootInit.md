---
title: "[#Spring] 기초 Spring Framework"
excerpt: "계속해서 작성해 나갈 Spring 기본 지식"

categories:
    - develop
# tags:
#     - [Blog, rhfy]

# toc: true   # 목차
# toc_sticky: true    #목차가 스크롤과 함께 이동

date: 2021-09-12
last_modified_at: 2021-09-28
---

1. Spring framework 란?
    1. Java 플랫폼을 위한 오픈소스 프레임워크
    2. 자바 엔터프라이즈 개발을 편하게 해주는 오픈 소스 경량급 프레임워크

2. 특징
    1. 경량 컨테이너로서 자바 객체를 직접 관리(IoC)
        1. 각각의 객체 생성, 소멸과 같은 라이프 사이클을 관리하며 스프링으로 부터 필요한 객체를 얻어온다
        2. 객체 생성, 소멸과 같은 라이프 사이클을 개발자가 아닌 프레임워크가 대신하여 제어권이 프레임워크로 넘어가기 때문에 이를 IoC(Inversion Of Control) 제어의 역전이라 한다
    2. POJO(Plain Old Java Object)
        1. 일반적인 J2EE 프레임워크에 비해 구현을 위하여 특정한 상속이나 구현이 필요하지 않는다.
        2. 기존에 존재하는 라이브러리 등을 지원하기에 용이하고 객체가 가벼움
    3. DI(Dependency Injection)
        1. 각각의 계층이나 서비스들 간에 의존성이 존재할 경우 프레임워크가 서로 연결
        2. 해당 부분이 IoC와 연관, 개발자가 의존성이 필요하다고 표시?하면 스프링이 의존성을 추가하여 준다.
        3. Autowired 어노테이션 사용(필드, 세터, 생성자 주입의 방법이 있음)
    4. AOP(Aspect-Oriented Programming)
        1. 관점지향 프로그래밍으로 로깅, 트랜젝션, 보안과 같은 동일한 기능(관점)의 경우 해당 기능을 분리하여 적용할 수 있다.
    5. 확장성이 높다
        1. Spring 진영은 수많은 라이브러리가 존재하고 레퍼런스가 다양하다

3. Bean객체를

4. MVC(model2)
    1. 컨트롤러와 뷰가 구분
    2. 호출 순서 : DispatcherServlet -> handlerMapping -> Controller -> Service -> Repository
    3. 응답순서는 2번 호출순서의 반대
