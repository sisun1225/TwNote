# 테스트

### 스프링 mvc 동작
DispatcherServlet 은 모든 연결을 담당하고 웹브라우저 요청이 들어오면 handlermapping 객체에게 컨트롤러 검색을 요청  
handlermapping은 클라이언트의 요청 경로를 이용해서 컨트롤러 객체를 찾고 DispatcherServlet 에게 리턴한다  
DispatcherServlet 은 @Controller 어노테이션을 이용해서 구현한 컨트롤러, HttpRequestHandler 인터페이스를 구현한 클래스를 처리하기위해 HandlerAdapter 객체에게 요청 처리를 위임한다.    
HandlerAdapter  객체는 컨트롤러의 알맞는 메소드를 호출해서 요청 처리하고 반환 결과물을 ModelAndView 객체에 담아서 DispatcherServlet 에 리턴한다  
ModelAndView 객체를 반환받은 DispatcherServlet 은 VIewResolver 객체를 이용해 결과를 보여줄 jsp 검색    
DispatcherServlet 은 ViewResolver  가 리턴한 view 객체에게 응답 결과를 생성을 요청  
jsp로 보여준다.  


