# Spring MVC란?

- Spring MVC는 Model2를 지칭한다.
- MVC란 Model - View - Controller 구조로 사용자 인터페이스와 비즈니스 로직을 분리하여 개발하는 것
- MVC에서는 Model1과 Model2로 나누어져 있다.
- **Model(모델)**
    - 데이터 처리를 담당하는 부분이고, Service 영역과 DAO영역으로 나누어지게 된다.
    - Model에서는 View와 Controller 어떠한 정보도 가지고 있어서는 안 된다.
- **View(뷰)**
    - View는 사용자 인터페이스를 담당하며 사용자에게 보이는 부분
    - Model이 가지고 있는 정보를 저장해서는 안되며 Model, Controller의 구성 요소를 알아선 안된다.
- **Controller(컨트롤러)**
    - Controller에서는 View에 받은 요청을 가공하여 Model(Service 영역)에 전달한다.
    - Model로부터 받은 결과를 View로 넘겨주는 역할을 하고, 모든 요청 에러와 모델 에러를 처리
    - Model과 View의 정보에 대해 알고 있어야 한다.
