다음 본문은 [실용주의 프로그래머](http://www.yes24.com/Product/Goods/12501565) 책 내용을 정리한 것입니다!  
작성자가 `마음에 드는 Tip`들만 모아서 정리했으니 **참고** 바랄게요~!  

### 깨진 창문을 내버려두지 말라

`깨진 창문` : 나쁜 설계, 잘못된 결정, 형편없는 코드  
절대로 **깨진 창문**을 고치지 않은채로 내버려 두지 마라!  
분명 언젠가는 **레거시 코드**가 될 운명이며 이는 `리팩토링` 대상이 될 게 뻔하다!  


### 변화의 촉매가 되라

무엇을 해야 하는지, 어떻게 해야 하는지 정확히 아는 상황이 있다  
시스템이 옳다는 걸 알지만 더 개선해볼 수 있다는 것을 안다  
하지만 `시작 피로`가 너무 과한 나머지 망설여질 때가 많다  
그럴때일수록 **사람들에게 보여줘라**  
"만약 ~를 추가하기만 하면 더 나아지겠죠" 처럼 안중요한 듯이 은근슬쩍 말해보자  


### 지식 포트폴리오에 주기적으로 투자하라

여러분의 지식 자산에 들어갈 최선의 길들은 몇가지가 있다
* 매년 새로운 언어를 최소 하나는 배워라
* 기술 서적을 분기마다 한 권씩 읽어라
* 비 기술 서적도 읽어라
* 수업을 들어라
* 지역 사용자 모임에 참여하라 -> 회사 밖에서도 다른 사람들이 어떤일 하는지 알아보라
* 다른 환경에서 실험해보라 -> 윈도우를 회사에서 쓰면, 집에서는 맥을!
* 요즘 흐름을 놓치지 마라
* 인터넷을 이용하라

### 무엇을 말하는가와 어떻게 말하는가 모두 중요하다

우리는 많은 `동료 프로그래머들`과 함께 일한다  
그만큼 커뮤니케이션은 중요하니까 말하기전에 **무엇을 말할지** 다시 한번 생각해보자  
말할 주제가 정해졌으면 **전달력 있게 말하는 것**도 능력이다  


### DRY원칙을 지키고 재사용하기 쉽게 만들어라

`DRY` : Don't Repeat Yourself, 중복은 정말 해악이다  
의사소통이든 코드든 중복은 업무의 효율성을 방해하는 요소다  
재사용하기 쉽게 만든다는 것은 남에게 `쉽게 잘 전달`되도록 작성하라는 의미다!  
아무리 좋은 코드나 문서라도 남이 잘 읽지 못하면 아무런 쓸모가 없다  


### 최종 결정이란 없다

소비자들의 요구는 끊임없이 변화한다  
세상이 변하는 만큼 실세계를 바탕으로 구현한 SW도 마찬가지로 계속 변한다  
특정 조건에 `의존적`으로 구현하게 되면 **변화에 느리게 대응**할 수 밖에 없다  
그러므로 항상 유연하게 코드 짜는 연습을 해라  


### 코드와 함께 일정도 반복하며 조정하라

우리는 `기한`을 지켜서 프로그램을 만드는 프로그래머다  
정확한 일정을 맞춰서 제작하는 것은 많이 어려울뿐더러 못지키면 `신뢰`만 잃을 뿐이다  
주로 우리가 고려해야되는 항목은
* 요구사항 체크하기
* 위험 분석하기
* 설계, 구현, 통합
* 사용자와 함께 검증하기
위 4가지 항목을 일정한 `반복주기`로 끊임없이 고려해야한다  
아직 정확한 추정을 모르는데 누군가 자꾸 물어본다면
```text
나중에 전화드릴게요
```
라고 말해라  


### 비난 대신 문제를 해결하라

버그가 여러분의 잘못인지 다른 사람의 잘못인지는 그리 중요한게 아니다  
어쨌거나 그 버그는 여러분의 문제로 남는다  
다른 사람의 문제를 해결해보자  
만약 여러분이 `단 하나`를 변경했고 시스템이 멈춘다면 `그 하나`가 문제가 있는 것이다  


### 가정하지 마라. 증명하라

놀라운 버그를 마주치면, 단순히 그걸 고치는 것을 넘어서 왜 이 `실패`가 더 일찍 발견되지 않았을까  
생각해볼 필요가 있다!  
마주친 버그와 동일한 버그가 있을 여지가 있는 다른 코드를 더 살펴봐라!!  
그리고 `팀`과 함께 공유해라. **한 사람이 그랬다는 것은 다른 사람도 충분히 잘못 작성할 수 있다**  


### 일찍 작동을 멈추게 하라

시스템이 문제가 있다면 절대로 그것을 감싸지 말고 `예외`로 멈추게 해라  
문제가 있는 시스템을 **유지**한다는 것이 더 바보 같은 생각이다  


### 모듈간의 결합도를 최소화하라

`디미터 함수 법칙` = 이 법칙은 한 객체가 제공하는 메서드에 접근하기 위해 또 다른 객체들을 통하는 것을 허용하지 않는다  
불필요한 **의존**이 많아질 수록 `시스템`은 **유지보수**하기 어렵다  

### 코드에는 추상화를, 메타데이터에는 세부 내용을

이렇게 하면 다음과 같은 이점이 있다
* 설계의 결합도를 줄여 좀 더 유연하고 적응성 있는 프로그램이 된다
* 세부사항을 코드 밖으로 몰아내서 강하고 추상적인 디자인을 만들 수 있다
* 애플리케이션을 커스터마이징 하기 위해 다시 컴파일할 필요가 없다
* 메타데이터는 범용 프로그래밍 언어보다 문제 도메인에 가까운 방식으로 표현할 수 있다


### 우연에 맡기는 프로그래밍을 하지 말라

우리는 매일마다 눈을 떠서 **코딩**을 한다  
그래서 그런지 코드를 작성하는 행위가 무의식적으로 하게 되는 기이한 현상을 경험할 수 있는데  
이는 매우 `위험`하다  
항상 **의도적**으로 프로그래밍하는 것이 좋다  
* 언제나 자기가 지금 무엇을 하고 있는지 알아야 한다
* 맹목적으로 코딩하지 말라
* 신뢰할 수 있는 것만 기대라
* 여러분의 가정을 문서로 남겨라
* 가정을 항상 테스트 하라
* 과거의 노예가 되지 말라
여기서 `실용주의 프로그래머 Tip`이 하나 포함되어 있다
```text
여러분의 가정을 테스트하고 문서로 남겨라
```

### 일찍 리팩터링하고, 자주 리팩터링 하라

리팩터링은 개발자의 `숙명`과도 같은 존재다  
레거시코드를 항상 **점진적으로 리팩토링**하는 연습을 해야 한다  
리팩토링을 하는 주요 대상은 다음과 같다
* 중복이 있을 떄
* 직교성이 좋지 않을 때
* 유효기간이 끝난 지식일 때
* 성능 이슈가 있을 때
`리팩터링`하면서는 절대 하지 말아야할 것이 있는데
```text
리팩터링과 동시에 새로운 기능 추가를 하지 마라
```


### 테스트를 염두에 두고 설계하라

이는 곧 `TDD`개발론과 일치하는 Tip이기에 자세한 설명은 생략한다  
테스트 코드는 `선택`이 아니라 `필수`다  
이와 비슷한 Tip으로는

### 일찍 테스트하고, 자주 테스트하라. 자동으로 테스트하라.

### 코드 커버리보다 상태 커버리지를 테스트하라

### 구체적인 것보다 추상적인 것이 더 오래간다

이는 `객체지향적인 설계`와 일치하는 부분이다  
객체간의 의존관계는 구체적인 것보다 `추상적`인 것에 의존해야 한다!  
예를 들자면, **직사각형**을 그린다고 가정했을 때 **직사각형**에 의존하지 말고 `도형`을 추상화해보라!  

### 생각의 틀을 벗어나지 말고, 틀을 찾아라

SW 개발자는 항상 의문점을 가지고 일을 해야 한다  
```text
반드시 이 방법으로 해야 하는가?
더 나은 방법은 없는가? 없다면 왜 없는가?
있다면 어떻게 나은건지 증명할 건가?
반드시 해야하는 일이긴 한가?
```
한걸음 뒤로 물러서서 스스로에게 끊임없이 `질문공세`를 해야 한다!  


### 형식적 방법의 노예가 되지 마라

시스템을 설계할 때 `UML 다이어그램`을 바탕으로 설계하고 이야기하는 경우가 많다  
*하지만 반드시 꼭 그래야 하는가?*  
아닐 수도 있다  
때로는 `코드`로 작성하는 것이 이해가 빠른 경우도 있고, `도식화`해서 이야기하는 것이 편한 경우가 있다  
```text
우리에겐 정답은 없다. 더 나은 방법을 택할 뿐
```

### 결국은 모두 글쓰기

```text
문서가 애초부터 전체의 일부가 되게 하고, 나중에 집어넣으려고 하지 말라
```
여러분이 작성한 API는 다른 동료들을 위하여 문서화할 필요가 있다  
하지만 주석에도 써야되지 말아야 할 것이 있으니
* 파일 내의 코드가 익스포트 하는 함수들의 목록
* 리비전 기록 -> git을 믿어라 제발
* 이 파일이 사용하는 파일 목록
* 파일 이름
