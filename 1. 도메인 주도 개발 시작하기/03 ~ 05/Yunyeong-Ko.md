### 1. 애그리거트의 특징에 대해 설명하세요.

<br>

### 2. 하나의 애그리거트로 묶이는 기준이 무엇인가요?

<br>

### 3. 애그리거트 루트에 대해 설명하세요.

<br>

### 4. 애그리거트와 JPA 매핑을 위한 기본 규칙은 무엇인가요?

<br>

### 5. CQBS는 무엇인가요?

<br>

### 6. 스펙은 무엇인가요?

<br>
<br>
<br>

답

---

1. 애그리거트는 일관성을 관리하는 기준이 되기 때문에 한 애그리거트에 속한 객체는 유사하거나 동일한 라이프 사이클을 갖습니다.

2. 기본적으로 도메인 규칙에 따라 함께 생성되고 변경되는 구성요소가 한 애그리거트에 속할 가능성이 높습니다.

3. 애그리거트 루트는 애거리거트에 속한 모든 객체를 관리하는 주체로서 일관성이 깨지지 않도록 합니다.

4. 애그리거트 루트는 엔티티이므로 @Entity로 매핑을 설정합니다.

5. 명령(Command)모델과 조회(Query)모델을 분리하는 패턴입니다.  
   명령 모델은 상태를 변경하는 기능을 구현할 때 사용되고, 조회 모델은 데이터를 조회하는 기능을 구현할 때 사용됩니다.

6. 스펙은 애그리거트가 특정 조건을 충족하는지를 검사할 때 사용하는 인터페이스입니다.
