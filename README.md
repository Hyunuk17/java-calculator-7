# java-calculator-precourse

---

### 기능 목록


#### 1. 문자열 입력 받기
- 문자열은 숫자(`0-9`) 또는 구분자(`,`,`:`, `커스텀 구분자`)로 이루어져 있다.
- 정상 입력을 받은 경우, 덧셈 연산 수행을 수행한다.
- 구분자가 연속으로 있다면, 사이에 `0`이 있다고 인식한다.

#### 2. 커스텀 구분자 사용
- 커스텀 구분자를 지정할 수 있다. 문자열 맨 앞의 `//`와 `\n` 사이에 위치한 문자를 구분자로 사용한다.
- 커스텀 구분자는 1자의 문자여야 한다.
- `//문자\n`

#### 3. 예외 처리
- 잘못된 입력을 받은 경우, `IllegalArgumentException`을 발생시킨 후 애플리케이션을 종료한다.
    - 문자열의 길이가 0(`empty`)인 경우
    - 구분자가 아닌 문자가 포함되어 있는 경우
    - 숫자가 음수(`-`)인 경우

#### 4. 숫자 추출하기
- 쉼표(`,`) 또는 콜론(`:`)을 포함한 문자열의 경우, 구분자로 활용하여 숫자를 분리한다.
- 커스텀 구분자를 이용하여 문자열을 분리할 수 있어야 한다.


#### 5. 덧셈 연산
- 연산 결과의 초기값은 0이다.
- 추출된 숫자를 전부 더한다.
- 피연산자(숫자)가 없으면, 0을 반환한다.

#### 6. 테스트
- 정상 흐름에 대한 테스트 케이스
- 커스텀 구분자 사용 시, 올바르게 수행되는지에 대한 테스트 케이스
- 잘못된 입력에 대한 올바른 예외처리 테스트 케이스
