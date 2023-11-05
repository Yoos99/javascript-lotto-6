# 로또

- 사용자는 원하는 만큼 로또를 구매하고 당첨 번호를 입력한다. 그 후 구매한 로때에 대하여 당첨 여부를 확인한다. 또한, 구입금액 대비 수익률을 알려준다.

## 기능 목록

- 사용자로부터 로또 구입 금액을 입력 받는다.
- 사용자로부터 당첨 번호, 보너스 번호를 입력 받는다.
- 로또 번호를 생성한다.
- 당첨 내역을 출력한다.
- 수익률을 계산한다.
- 사용자가 잘못된 값을 입력할 경우 throw문을 사용해 예외를 발생시킨다.

```
  - 1,000원으로 나누어 떨어지지 않는 금액 입력
  - 숫자가 아닌 문자열 입력
  - 1~45의 숫자가 아닌 로또 번호
  - 로또 번호에 중복된 숫자 존재
  - 로또 번호가 6개를 초과
```

---

## 🚀 기능 요구 사항

- 로또 게임 기능을 구현해야 한다. 로또 게임은 아래와 같은 규칙으로 진행된다.

```
- 로또 번호의 숫자 범위는 1~45까지이다.
- 1개의 로또를 발행할 때 중복되지 않는 6개의 숫자를 뽑는다.
- 당첨 번호 추첨 시 중복되지 않는 숫자 6개와 보너스 번호 1개를 뽑는다.
- 당첨은 1등부터 5등까지 있다. 당첨 기준과 금액은 아래와 같다.
    - 1등: 6개 번호 일치 / 2,000,000,000원
    - 2등: 5개 번호 + 보너스 번호 일치 / 30,000,000원
    - 3등: 5개 번호 일치 / 1,500,000원
    - 4등: 4개 번호 일치 / 50,000원
    - 5등: 3개 번호 일치 / 5,000원
```

- 로또 구입 금액을 입력하면 구입 금액에 해당하는 만큼 로또를 발행해야 한다.
- 로또 1장의 가격은 1,000원이다.
- 당첨 번호와 보너스 번호를 입력받는다.
- 사용자가 구매한 로또 번호와 당첨 번호를 비교하여 당첨 내역 및 수익률을 출력하고 로또 게임을 종료한다.
- 사용자가 잘못된 값을 입력할 경우 `throw`문을 사용해 예외를 발생시킨다. 그런 다음, "[ERROR]"로 시작하는 에러 메시지를 출력하고 해당 부분부터 입력을 다시 받는다.
  ```
  예시) [ERROR] 숫자가 잘못된 형식입니다.
  ```