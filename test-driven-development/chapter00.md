# 테스트 주도 개발 - 저자의 글

```text
created: 2020-09-15 00:09:43
updated: 2020-09-15 00:09:43
```

```text
<Quiz>
  1. TDD를 하는 이유에 대해서 말하시오.
  2. TDD 사이클에 대해서 말하시오
  3. TDD를 통해 무엇을 얻을 수 있는지 말하시오.
</Quiz>
```

## 시작하기

저자의 글에서 마음에 와닿는 글들이 많았다.

몇가지 적어보자.

TDD의 궁극적 목표는 `작동하는 깔끔한 코드`를 만드는 것이다.

이를 목표를 도달 했을 때, 다음과 같은 이점이 있다.

- 예측 가능한 개발 방법
- 리팩토링을 통해서 학습할 기회를 갖게 됨(예로 테스트 코드를 작성함에 따라서 리팩토링 단계에서 한 번 더 생각하는 시간을 가지게 되어서 학습할 기회를 가진다고 생각하고 있음)
- 사용자의 삶을 향상시켜준다.(이건 아직 잘 와닿지 않는다.)
- 동료들이 존경해준다.
- 작성하는 동안 기분이 좋다.(어려워서 멘붕에 빠져있는 내모습..)

## TDD의 단순한 규칙

- 자동화된 테스트가 실패할 경우에만 새로운 코드를 작성
- 중복을 제거

> 이건 아주 많이 고민 되는 부분 중하나인데, 응집도는 높고 결합도는 낮은 컴포넌트를 구성하는 건 어렵다.ㅠㅠ

## R G B

빨강 - 초록 - 블루 사이클로 돌아가는 TDD방법!

실패하는 작은 테스트를 작성하고

빨리 테스트가 통과하게끔 만들고

테스트를 통과하면 중복을 제거하고 개선해본다.

## 그러면 왜 TDD를 해야되나

왜 우리는 자동화된 테스트를 만드느라 시간을 할애해야되는지가 의문!

그 이유는 용기라고 한다.

TDD에선 멘탈 관리가 중요하다고 한다.

만약 TDD하면서 두려움이 생기게 되면 다음과 같은 일이 일어날 수도 있다.

- 망설이게 됨
- 커뮤니케이션을 덜하게 됨
- 피드백 받는 것을 피하도록 만듬

이러한 건 도움 되지 않는다.

그래서 우리는

- 불확실한 상태로 있기 보다는 구체적인 학습을 빠르게 시작해야함
- 침묵 대신 많은 커뮤니케이션을 해야함
- 구체적인 피드백을 찾아야함

## 그래서 나는

나에게 TDD를 왜 하냐고 물어봤을 때

나는 `피드백을 빠르게 받기 위함`이라고 말하고 있었는데,

또 추가적인 이유가 생겨서 좋았다.

그 중에서 가장 마음에 와닿는 부분이 학습을 다시 하게 된다는 부분인 것 같다.

리팩토링을 하면서 한 번 더 생각하는게 중요한 것 같다.

어떻게 하면 중복을 제거할 수 있을까?

어떻게 하면 컴포넌트 간의 관심사를 분리할 수 있을까?

테스트는 어디까지 커버해야할까? 등등 고민하게 된다.

TDD는 어렵지만, 가치있는 일임에 몸소 체감해간다.