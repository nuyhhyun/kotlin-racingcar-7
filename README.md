# 🏎 kotlin-racingcar-precourse 🏎

> 초간단 자동차 경주 게임을 구현한다.
***

## ❗️요구 사항

- **주어진 횟수** 동안 **n대**의 자동차는 **전진 또는 멈출** 수 있다.
- 각 자동차에 **이름을 부여**할 수 있다.
  - **전진**하는 자동차를 출력할 때 자동차 **이름을 같이 출력**한다.
    - 예:
      ```
      실행 결과
      pobi : --
      woni : ----
      jun : ---
      
      pobi : --
      woni : -
      jun : --
      
      pobi : ---
      woni : --
      jun : ---
      
      pobi : ----
      woni : ---
      jun : ----
      
      pobi : -----
      woni : ----
      jun : -----
      ```
- **자동차 이름은 쉼표(,)를 기준으로 구분**하며 **이름은 5자 이하**만 가능하다.
  - 예:
    ```
    경주할 자동차 이름을 입력하세요.(이름은 쉼표(,) 기준으로 구분)
    pobi,woni,jun
    ```
- 사용자는 **몇 번의 이동을 할 것인지를 입력**할 수 있어야 한다.
  - 예:
    ```
    시도할 횟수는 몇 회인가요?
    5
    ```
- **전진하는 조건**은 **0에서 9 사이에서 무작위 값**을 구한 후 무작위 값이 **4 이상**일 경우이다.
- 자동차 경주 게임을 완료한 후 **누가 우승했는지를 알려준다**.
  - 예: `최종 우승자 : pobi`
  - 우승자는 **한 명 이상**일 수 있다.
    - 예: `최종 우승자 : pobi, jun`
- **우승자**가 여러 명일 경우 **쉼표(,)를 이용하여 구분**한다.
- 사용자가 **잘못된 값을 입력**할 경우 `IllegalArgumentException`을 발생시킨 후 애플리케이션은 종료되어야 한다.

## ✅ 기능 명세

### 입력
- [X] 경주할 자동차 이름들을 담은 문자열을 입력할 수 있다.
  - [X] 자동차는 두 대 이상 입력해야 한다.
- [X] 시도 횟수를 입력할 수 있다.

### 출력
- [ ] 경주할 자동차 입력을 안내할 수 있다.
- [ ] 시도 횟수 입력을 안내할 수 있다.
- [ ] 경기의 진행 상황을 출력할 수 있다.
- [ ] 우승자를 출력할 수 있다.

### 자동차
- [ ] 자동차에 이름을 부여할 수 있다.
  - [ ] 자동차 이름은 5자 이하이어야 한다.
- [ ] 자동차는 본인의 위치를 가질 수 있다.
    - [ ] 무작위 값이 4 이상인 경우 전진하고 아니면 멈춰있는다.

### 차고지
- [ ] 쉼표(,)를 기준으로 각 자동차 이름을 구분할 수 있다.
- [ ] 경주할 자동차들의 대수를 셀 수 있다.

### 경주
- [ ] 시도 횟수만큼 경주를 진행할 수 있다.
    - [ ] 각 시도마다 각 자동차의 이름과 전진한 횟수만큼의 붙임표(-)를 함께 알려준다.
- [ ] 우승자를 구할 수 있다.
  - [ ] 우승자가 여러 명일 경우 쉼표(,)를 이용하여 우승자를 구분한다.

### 무작위 값
- [ ] 0에서 9 사이에서 무작위 값을 구할 수 있다.

### 시도 횟수
- [ ] 시도 횟수는 양의 정수이어야 한다.

### 예외
- [ ] 사용자가 잘못된 값을 입력한 경우 `IllegalArgumentException`을 발생시킨 후 애플리케이션을 종료시킬 수 있다.