### 블로그 주소 : https://velog.io/@woongbin06/DDD-%EB%8F%84%EB%A9%94%EC%9D%B8-%EC%A3%BC%EB%8F%84-%EA%B0%9C%EB%B0%9C-Chapter-1-2

<br>

### 1. 도메인이란 무엇이고 무엇으로 구성되어있나요?
<br>

### 2. 어플리케이션의 아키텍처는 몇 개의 영역으로 구성되고, 영역들의 이름이 무엇인가요?
<br>

### 3. 도메인을 모델링할 때 기본이 되는 작업들은 무엇인가요?
<br>

### 4. 엔티티에서 set 메서드를 넣으면 안되는 이유는 무엇인가요?
<br>

### 5. 도메인 용어를 사용하여 코드를 작성해야 하는 이유는 무엇인가요?

### 6. 인프라스트럭처에 의존하게 되면 발생하는 문제 두 가지는 무엇이고, 무엇을 이용하여 해결할 수 있나요?
<br>

### 7. 애그리거트가 무엇이고 애그리거트 안에 있는 객체들을 관리하는 엔티티를 어떤 엔티티라고 부르나요?

<br>
<br>
<br>

답
<hr>

1. 도메인은 소프트웨어로 해결하고자 하는 문제영역이다. 도메인은 여러개의 하위 도메인으로 구성되어 있다.

2. 4개의 영역으로 구성되고 표현, 응용, 도메인, 인프라스트럭처 영역이다.

3. 도메인이 모델링할 대 기본이 되는 작업은 핵심 구성요소, 규칙, 기능을 찾는 것이다.

4. set 메서드는 도메인의 핵심 개념이나 의도를 코드에서 사라지게 하기 때문이다.   
또는  도메인 객체를 생성할 때 온전하지 않은 상태가 될 수 있기 때문이다.

5. 코드를 도메인 용어로 해석하는 과정 줄어들기 때문이다.   
또는 가독성을 높여 코드를 분석하고 이해하는 시간이 줄어들기 때문이다.   
또는 도메인 규칙으로 코드를 작성하기 때문에 버그를 줄여주기 때문이다.

6. 테스트가 어렵고 기능 확장이 어려워진다는 문제가 있다. DIP를 이용하여 해결할 수 있다.

7. 애그리거트는 연관된 엔티티와 밸류 객체를 개념적으로 하나로 묶은 것이다. 루트 엔티티라고 부른다.