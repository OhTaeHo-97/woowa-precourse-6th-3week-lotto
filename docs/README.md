# 📋 기능 요구 사항
## 1️⃣ 입력
- [ ] 로또 구입 금액을 입력받는다.
    - [ ] 1,000원 단위로 입력받는다.
- [ ] 당첨 번호를 입력받는다.
    - [ ] 쉼표를 기준으로 구분하여 입력받는다.
    - [ ] 1 ~ 45 사이의 숫자를 입력받는다.
    - [ ] 6개의 숫자를 입력받는다.
    - [ ] 중복되지 않은 숫자를 입력받는다.
- [ ] 보너스 번호를 입력받는다.
    - [ ] 1 ~ 45 사이의 숫자를 입력받는다.
    - [ ] 당첨 번호와 중복되지 않는 숫자를 입력받는다.

## 2️⃣ 출력
- [ ] 구매한 로또 개수를 출력한다.
- [ ] 로또 번호를 출력한다.
    - [ ] 로또별로 한 줄씩 출력한다.
    - [ ] 로또 번호를 오름차순으로 정렬하여 출력한다.
    - [ ] 형식: [로또 번호들] (ex. [8, 21, 23, 41, 42, 43])
- [ ] 당첨 통계를 출력한다.
    - [ ] 5등부터 1등까지 당첨된 로또 개수를 출력한다.
    - [ ] 수익률을 소수점 둘째 자리에서 반올림하여 출력한다. (수익률 = 수익 / 구매 금액 * 100)

## 3️⃣ 로또 게임
### 시작
- 구입 금액
    - [ ] 구입 금액 입력을 위한 문구를 출력한다.
    - [ ] 구입 금액을 입력받는다.
- 구매한 로또 개수
    - [ ] 구입 금액에 맞는 구매한 로또 개수를 구한다.
    - [ ] 구매한 로또 개수를 출력한다.
- 로또 번호
    - [ ] 각 로또별 로또 번호를 생성한다.
    - [ ] 로또 번호를 출력한다.
- 당첨 번호 및 보너스 번호
    - [ ] 당첨 번호 입력을 위한 문구를 출력한다.
    - [ ] 당첨 번호를 입력받는다.
    - [ ] 보너스 번호 입력을 위한 문구를 출력한다.
    - [ ] 보너스 번호를 입력받는다.

### 로또 게임 진행
- [ ] 1등부터 5등까지 당첨된 로또 개수를 구한다.
- [ ] 당첨된 로또 개수를 기반으로 수익을 구한다.
- [ ] 수익률을 구한다.

### 경주 종료
- [ ] 당첨 통계를 출력한다.

## 4️⃣ 예외 처리
- 로또 구입 금액을 입력받는다.
    - [ ] null을 입력하면 IllegalArgumentException을 발생시킨다.
    - [ ] 빈 문자열을 입력하면 IllegalArgumentException을 발생시킨다.
    - [ ] 숫자가 아니라면 IllegalArgumentException을 발생시킨다.
    - [ ] 1,000원 단위로 입력하지 않으면 IllegalArgumentException을 발생시킨다.
- 로또 번호를 생성한다.
    - [ ] 6개의 숫자가 아니라면 IllegalArgumentException을 발생시킨다.
    - [ ] 중복된 숫자가 존재하면 IllegalArgumentException을 발생시킨다.
- 당첨 번호를 입력받는다.
    - [ ] null을 입력하면 IllegalArgumentException을 발생시킨다.
    - [ ] 빈 문자열을 입력하면 IllegalArgumentException을 발생시킨다.
    - [ ] 쉼표를 기준으로 6개의 번호가 입력되지 않았다면 IllegalArgumentException을 발생시킨다.
    - [ ] 각 번호가 숫자가 아니라면 IllegalArgumentException을 발생시킨다.
    - [ ] 1 ~ 45 사이의 숫자가 아니라면 IllegalArgumentException을 발생시킨다.
    - [ ] 중복된 숫자가 존재한다면 IllegalArgumentException을 발생시킨다.
- 보너스 번호를 입력받는다.
    - [ ] null을 입력하면 IllegalArgumentException을 발생시킨다.
    - [ ] 빈 문자열을 입력하면 IllegalArgumentException을 발생시킨다.
    - [ ] 숫자가 아니라면 IllegalArgumentException을 발생시킨다.
    - [ ] 1 ~ 45 사이의 숫자가 아니라면 IllegalArgumentException을 발생시킨다.
    - [ ] 당첨 번호와 중복된 숫자라면 IllegalArgumentException을 발생시킨다.

---

# 📂 도메인별 기능 정리

## 🙎‍♂️ 로또 게임 플레이어(Player)
- [ ] 수익률을 계산할 수 있다.
    - [ ] 소수점 둘째 자리에서 반올림한다.

## 🕹️ 로또 게임(LottoGame)
- [ ] 로또 구입 금액을 입력받을 수 있다.
    - [ ] 1,000원 단위로 입력받는다.
- [ ] 당첨 번호를 입력받을 수 있다.
    - [ ] 쉼표를 기준으로 구분하여 입력받는다.
    - [ ] 1 ~ 45 사이의 숫자를 입력받는다.
    - [ ] 6개의 숫자를 입력받는다.
    - [ ] 중복되지 않은 숫자를 입력받는다.
- [ ] 보너스 번호를 입력받을 수 있다.
    - [ ] 1 ~ 45 사이의 숫자를 입력받는다.
    - [ ] 당첨 번호와 중복되지 않는 숫자를 입력받는다.
- [ ] 1등부터 5등까지 당첨된 로또 개수를 구할 수 있다.
- [ ] 당첨된 로또 개수를 기반으로 수익을 구할 수 있다.
- [ ] 당첨 통계를 출력할 수 있다.

## 📝 로또(Lotto)
- [ ] 구입 금액에 맞는 구매한 로또 개수를 구할 수 있다.
- [ ] 로또 번호를 생성할 수 있다.
    - [ ] 6개의 숫자를 생성한다.
    - [ ] 1 ~ 45 사이의 숫자를 생성한다.
    - [ ] 중복된 숫자는 허용하지 않는다.