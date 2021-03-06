### 목적

> 이번 프로젝트의 주 목적
1. 실제 서비스와 같은 정도의 수준으로 개발을 진행한다.   
2. Gradle을 사용한다. (공식 홈페이지 기준, DI가 커지면 커질수록 성능차이가 남.)   
3. application.properties 가 아닌 application.yml을 사용한다.   
4. 최근에 읽은 도서인 Clean Code에서 학습한 내용을 바탕으로 개발한다.

## h2
> h2/bin/./h2.shf
> localhost:8082


## Content
> ㄷㅏ이어리 작성해서 crontab + batch


### Additional 
> Clean Code 정리

> 주석
>> 부적절한, 쓸모 없는, 중복 된, 성의 없는 주석은 필요 없음.   
>
>환경
>> 여러 단계로 빌드와 테스트를 거친다.   
>
>함수
>> 적은 입/출력과 인수/플래그를 사용.   
>> 올바른 위치에 선언되게끔 시간을 들여 고민.   
>> True / False 보다 정확한 Return을 줄 것.   
>
>일반
>> 한 소스에 여러 언어 지양.   
>> 예외처리, 절차 중요.   
>> 중복제거, 죽은 코드, 비어있는 생선자는 시스템에서 제거.   
>> 올바른 추상화 단계 (고 차원개념/ 저 차원개념 구분.)   
>> 올바른 의존 관계 (기초 클래스가 파생 클래스에 의존하지 않음.)   
>> 캡슐화(매우 적고 간단하면서, 정보를 제한.)를 통해 결합도를 낮춤.   
>> 사용하기 직전에 선언하여 변수와 함수의 수직 분리.내려가기 규칙.(책 읽는 것 처럼 읽혀야한다.)         
>> 최소놀람의 법칙. ( 아니 이게 왜 여기서 나와? 즉 일관성 유지.)   
>> 참조/변경 시 다른 클래스나 함수말고, 자신 클래스에서 해결할 것.      
>> 코드에 "분명한 의도"를 줄 것.   
>> 마주잡이 static 함수 사용 금지.   
>> 서술적 변수 사용, 이름과 기능이 일치하는 함수.   
>> 알고리즘의 이해.    
>> 논리적 의존성은 물리적으로 드러낼 것.   
>> If/Else, switch/Case 보다 다형성 사용.      
>> 매직 숫자는 명명된 상수로 교체. (코드에서 숫자를 사용 하지 말것.)   
>> 관례보다 구조를 사용.   
>> 조건보다 캡슐화.   
>> 부정 조건보다 긍정 조건.   
>> 함수 내 명령과 조회를 다른 함수로 분리하여 함수는 1가지의 기능만 하도록.   
>> 숨겨진 시간적인 결합.???   
>> 경계조건 캡슐화.   
>> 함수는 추상화 수준을 한 단계만 내려가서 수준을 유지.   
>> 설정 정보는 최상위 단계.   
>> 추이적 탐색 회피. 즉, a.get().b.get().c.get()..같은 한 모듈은 주변 모듈을 모르면 모를 수록 좋다.   
>> 
> Java
>> 여러 import 보다 .*(와일드카드) 사용.   
>> 상수는 상속하지말고, 상속보다는 Enum을 사용.   
>> 서술적이고 명확한 이름 사용.   
>> 적절한 추상화 수준에서 이름 선택.   
>> 범위만큼의 이름 사용. (이름의 길이는 범위 길이에 비례.)   
>> 인코딩 회피.(이름에 유형 정보나 범위 정보 넣지 말 것.)
>> 이름으로 부수 효과를 설명.
>> 클래스는 명사구, 메서드는 동사구.     
>> 
>> 함수 내 명령과 조회를 다른 함수로 분리.   
>> 오류보다 예외를 이용.   
>> null 을 반환하지 말 것.   
>> 객체는 동작을 공개하고, 자료는 숨김.   
>> 경계 구분 철저히.(어디부터 어디까지 동작하는지.)   
>>
>
> Test
>> 충분한 테스트와 커버리지 도구를 사용.   
>> 사소한 테스트도 건너뛰지 말 것.   
>> 무시한 테스트는 잠재적 폭탄.   
>> 예외 조건 테스트.
>> 버그 주변은 또 다른 버그가능성 높음.   
>> 실패 패턴과 테스트 커버리지 패턴을 살필 것.      
>> 테스트는 빨라야 함.   
>> 단위 테스트는 재사용성을 높힌다.(수정 시 재확인이 빠르다.)
>




경계를 구분을 철저히 (내 코드가, 어디부터 어디까지 동작하는지. 다른 코드와의 경계를 뜻. 이 구간에서의 테스트도 중요)
단위테스트는 재사용성을 높인다. 수정되더라도 재확인이 빠르다.
-> 수정 후 단위테스트 -> 수정 ->테스트(모든예외가 확인됨.)
모든 테스트를 실행한다.
중복을 없앤다.
코드에서 의도를 표현한다.
클래스,메서드 수를 최소로 줄인다.






