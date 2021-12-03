# 미션 - 자동차 경주 게임

---

## 🔍 프로젝트를 하며 고민했던 부분 


## 🚀 구현할 기능 목록

---

> ### 1. 입력

- ### 자동차 이름 목록
  - [ 예외 ] : `공백`
  - [ 예외 ] : 자동차가 `2대 미만`
  - [ 예외 ] : 이름이 `중복`
  - [ 예외 ] : `5글자 초과`


- ### 시도할 횟수 
  - [ 예외 ] : 숫자가 아닌 `문자` 
  - [ 예외 ] : `1 미만`
    

- ### 예외 처리
  - `IllegalArgumentException`를 발생 시킴
  - `[ERROR]`로 시작하는 에러 메시지를 출력
  - 에러 생성 지점부터 `다시 입력 받음 ` 
  


> ### 2. 레이싱 

- ### 자동차 이동
  - `0에서 9 사이에서 무작위 값을 구한 후` 무작위 값이 `4 이상일 경우 전진`
    - 입력 받은 횟수 만큼 이동 시도
  - 개별 자동차 위치 갱신
  
  
- ### 경기 진행
  - 입력 받은 `횟수 만큼 반복해서 경기 진행`
  - 경기 별 우승자 판별 
  - 최종 우승자 판별



> ### 3. 출력

- ### 각 차수별 실행 결과
  - `이름 : 이동한 거리 * ( - ) 로 출력`
- ### 최종 우승자 
  - `단독` 우승자
  - `공동` 우승자 
    - "," 로 분리하여 출력


----


### 프로그래밍 요구사항 - Randoms, Console

- JDK에서 기본 제공하는 Random, Scanner API 대신 `camp.nextstep.edu.missionutils`에서 제공하는 `Randoms`, `Console` API를 활용해 구현해야 한다.
   - Random 값 추출은 `camp.nextstep.edu.missionutils.Randoms`의 `pickNumberInRange()`를 활용한다.
   - 사용자가 입력하는 값은 `camp.nextstep.edu.missionutils.Console`의 `readLine()`을 활용한다.
- 프로그램 구현을 완료했을 때 `src/test/java` 디렉터리의 `ApplicationTest`에 있는 모든 테스트 케이스가 성공해야 한다. **테스트가 실패할 경우 0점 처리한다.**

<br>

---

## 📈 과제 진행 요구사항

- 미션은 [java-racingcar-precourse](https://github.com/woowacourse/java-racingcar-precourse) 저장소를 Fork/Clone해 시작한다.
- **기능을 구현하기 전에 java-racingcar-precourse/docs/README.md 파일에 구현할 기능 목록을 정리**해 추가한다.
- **Git의 커밋 단위는 앞 단계에서 README.md 파일에 정리한 기능 목록 단위**로 추가한다.
   - [AngularJS Commit Message Conventions](https://gist.github.com/stephenparish/9941e89d80e2bc58a153) 참고해 commit log를 남긴다.
- 과제 진행 및 제출 방법은 [프리코스 과제 제출 문서](https://github.com/woowacourse/woowacourse-docs/tree/master/precourse) 를 참고한다.

<br>

---

## 📝 License

This project is [MIT](https://github.com/woowacourse/java-racingcar-precourse/blob/master/LICENSE) licensed.
