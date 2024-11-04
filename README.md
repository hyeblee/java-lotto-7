# 🎯 기능 구현 목록

### 1️⃣ 로또 구입 금액 입력
- **구입 금액 입력 안내**: 사용자에게 구입 금액 입력을 요청 :ballot_box_with_check:
- **구입 금액 입력 및 검증**:
  - 문자열로 입력받아 숫자로 변환 :ballot_box_with_check:
  - 변환 실패 시, `[ERROR] 유효한 정수를 입력해주세요.` 예외 메시지 출력 :ballot_box_with_check:
  - 양수가 아닐 경우, `[ERROR] 양수만 입력할 수 있습니다.` 예외 메시지 출력 :ballot_box_with_check:
  - **1000원 단위 금액인지 검증**:
    - 1000원 단위가 아닐 시, `[ERROR] 구입금액은 1000 :ballot_box_with_check:원 단위여야 합니다.` 예외 메시지 출력 :ballot_box_with_check:
  - **올바른 금액 입력 시**까지 반복 요청



### 2️⃣ 로또 구입
- **로또 수량 계산**: 구입 금액에 따라 구매할 로또 수량 계산 :ballot_box_with_check:
- **로또 구매 수량 출력** :ballot_box_with_check:



### 3️⃣ 로또 번호 발행
- **로또 번호 생성**:
  - 6개의 랜덤 번호 생성(범위는 1~45) :ballot_box_with_check:
  - 6개의 번호 오름차순 정렬 :ballot_box_with_check:
  - 구입한 로또 갯수만큼 반복하여 번호 생성 :ballot_box_with_check:
  - 생성 결과 출력



### 4️⃣ 당첨 번호 입력
- **당첨 번호 입력 안내**: 사용자에게 당첨 번호 입력을 요청
- **당첨 번호 입력 및 검증**:
  - 한 줄의 문자열로 당첨 번호 입력
  - `,`를 기준으로 분리
  - 각 요소를 숫자로 변환
  - 변환 실패 시, `[ERROR] 숫자를 입력해주세요.` 예외 메시지 출력
  - **1부터 45 사이의 숫자인지 검증**:
    - 범위를 벗어날 경우, `[ERROR] 번호는 1부터 45 사이의 숫자여야 합니다.` 예외 메시지 출력
  - **번호가 6개인지 검증**:
    - 6개가 아니라면, `[ERROR] 로또 번호는 6개여야 합니다.` 예외 메시지 출력
  - **올바른 번호 입력 시**까지 반복 요청



### 5️⃣ 보너스 번호 입력
- **보너스 번호 입력 안내**: 사용자에게 보너스 번호 입력을 요청
- **보너스 번호 입력 및 검증**:
  - 번호스 번호 입력
  - 입력받은 값을 숫자로 변환
  - 변환 실패 시, `[ERROR] 숫자를 입력해주세요.` 예외 메시지 출력
  - **1부터 45 사이의 숫자인지 검증**:
    - 범위를 벗어날 경우, `[ERROR] 번호는 1부터 45 사이의 숫자여야 합니다.` 예외 메시지 출력
  - **올바른 보너스 번호 입력 시**까지 반복 요청



### 6️⃣ 당첨 결과 확인
- **로또 번호와 당첨 번호 비교**:
  - 각 로또의 당첨 번호와 일치하는 갯수 카운트
  - 5개 일치 시, 보너스 번호 포함 여부 확인
- **당첨 통계 계산 및 출력**:
  - 당첨 통계 계산
  - 당첨 통계 출력



### 7️⃣ 수익률 계산
- **수익률 계산 및 출력**:
  - 구입 금액 대비 수익률 계산
  - 수익률 출력
