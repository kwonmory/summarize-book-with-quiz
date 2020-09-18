# 다중 통화를 지원하는 Money객체

```text
created: 2020-09-15 14:09:43
updated: 2020-09-15 14:09:43
```

```text
<Quiz>
  1. TDD의 순서 말하기
  2. 오퍼레이션이란 무엇인가
  3. 스텁이란 무엇인가
  4. 리팩토링의 의미는 무엇인가
</Quiz>
```

## 시작하기

시작부터 TDD의 순서를 이야기했다.

1. 재빨리 테스트를 하나 추가
2. 모든 테스트를 실행하고 실패를 확인
3. 코드가 테스트를 통과할 수 있게 수정
4. 리팩토링으로 중복 제거

보면서 오퍼레이션에 대한 개념을 알게되었다.

> 오퍼레이션

설명 글에서는 메서드와 비슷한 의미로 객체가 수행할 수 있는 연산을 의미한다고 한다.

그냥 동작이라고 생각해도 무방할 것 같다.

## 테스트 대상 찾기

테스트 대상을 선택할 때, 오퍼레이션이 외부에서 어떤 식으로 보일지에 대해서 생각해봐야한다.

책에서는 화폐를 예로들어 TDD를 수행하는 과정들을 소개해준다.

그 중 메서드는 스텁 구현을 통해서 처리를 우선적으로 하는 부분이 매력적이다.

> 스텁 구현

스텁 구현은 메서드의 서명부와 반환 명령만 적는 식이라고 한다. 그래서 이 메서드를 호출하는 코드는 컴파일이 될 수 있도록 껍데기만 만들어두는 것이라고 한다.

그 전까지는 스텁이라는게 그냥 목킹이라고 생각했는데, 약간 차이가 있나보다.

> 리팩토링

리펙토링 등장하게 되는데, 리팩토링이란게 단순하게 기존 코드를 좋은 코드로 수정한다라고 알고 있었는데, 정확한 의미는 코드의 외적 행위는 그대로 유지하면서 내부 구조를 바꾸는 작업을 말한다고 한다.

## 의존성과 중복

TDD를 하면서 항상 의문이 들었던 건 어떤 중복을 제거하고 서로 의존하는 부분을 어떻게 제거하는가가 많은 고민이였다.

일단은 중복만 제거해주면 의존성도 제거해준다고 하니 중복을 어떻게 어떤걸 제거해야되는지 많이 생각해보자.

중복이라고 함은 보통 코드가 동일한 부분을 찾게 되는데, 그게 아니라 의미적으로 어떤 부분이 다른 걸로 대체될 수 있다고 하면 중복이라고 인식해도 좋을 것 같다.