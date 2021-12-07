# 🚘︎ 미션 - 자동차 경주 게임 🚘︎

---
## 💁‍♀ 게임 설명
```
안녕하세요. 이 프로젝트는 우아한테크코스 4기 2주차 미션을 진행합니다. 😛

자동차 이름(최소 2개 이상)과 반복 횟수(최대 이동 거리)를 입력받고, 

반복 횟수 만큼 0~ 9 사이의 랜덤 넘버를 생성하여 4이상이면 전진, 미만이면 정지하여

최종적으로 어떤 자동차가 제일 멀리갔는지, 레이싱의 승자를 찾는 게임입니다. 

게임이 종료되면, 진행 과정과 최종 승자가 출력됩니다. 
```

---

## 🔍 프로젝트를 하며 고민했던 부분 
- [NsTest 클래스에 메서드를 파악해보자! ](https://github.com/her0807/java-racingcar-precourse/wiki/NsTest-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%97%90-%EB%A9%94%EC%84%9C%EB%93%9C%EB%A5%BC-%ED%8C%8C%EC%95%85%ED%95%B4%EB%B3%B4%EC%9E%90.)
- [객체 지향적인 설계는 어떻게 할까?](https://github.com/her0807/java-racingcar-precourse/wiki/%EA%B0%9D%EC%B2%B4-%EC%A7%80%ED%96%A5%EC%A0%81%EC%9D%B8-%EC%84%A4%EA%B3%84%EB%8A%94-%EC%96%B4%EB%96%BB%EA%B2%8C-%ED%95%A0%EA%B9%8C%3F)
- [객체 지향적인 자동차 경주 설계](https://github.com/her0807/java-racingcar-precourse/wiki/%EA%B0%9D%EC%B2%B4-%EC%A7%80%ED%96%A5%EC%A0%81%EC%9D%B8-%EC%9E%90%EB%8F%99%EC%B0%A8-%EA%B2%BD%EC%A3%BC-%EA%B2%8C%EC%9E%84-%EC%84%A4%EA%B3%84)
- [Getter / Setter 를 쓰지 말아야하는 이유가 뭘까?](https://github.com/her0807/java-racingcar-precourse/wiki/Getter---Setter--%EB%A5%BC-%EC%93%B0%EC%A7%80-%EB%A7%90%EC%95%84%EC%95%BC%ED%95%98%EB%8A%94-%EC%9D%B4%EC%9C%A0%EA%B0%80-%EB%AD%98%EA%B9%8C%3F)
- [좋은 네이밍이란 무엇일까?](https://github.com/her0807/java-racingcar-precourse/wiki/%EC%A2%8B%EC%9D%80-%EB%84%A4%EC%9D%B4%EB%B0%8D%EC%9D%B4%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%BC%EA%B9%8C%3F)
- ["pobi, jun," 을 String.split(",") 으로 분할하면 배열의 크기는 3일까?](https://github.com/her0807/java-racingcar-precourse/wiki/%22pobi,-jun,%22-%EC%9D%84--String.split(%22,%22)-%EC%9C%BC%EB%A1%9C-%EB%B6%84%ED%95%A0%ED%95%98%EB%A9%B4--%EB%B0%B0%EC%97%B4%EC%9D%98-%ED%81%AC%EA%B8%B0%EB%8A%94-3%EC%9D%BC%EA%B9%8C%3F)
- [의존성 주입이란?](https://github.com/her0807/java-racingcar-precourse/wiki/%EC%9D%98%EC%A1%B4%EC%84%B1-%EC%A3%BC%EC%9E%85%EC%9D%B4-%EB%AD%98%EA%B9%8C%3F-%EC%99%9C-%EC%82%AC%EC%9A%A9%ED%95%A0%EA%B9%8C%3F)
- [스트림이 뭘까?](https://github.com/her0807/java-racingcar-precourse/wiki/%EC%8A%A4%ED%8A%B8%EB%A6%BC%EC%9D%B4-%EB%AD%98%EA%B9%8C%3F)

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


###  수행한 프로그래밍 요구사항 - Randoms, Console

- JDK에서 기본 제공하는 Random, Scanner API 대신 `camp.nextstep.edu.missionutils`에서 제공하는 `Randoms`, `Console` API를 활용해 구현해야 한다.
   - Random 값 추출은 `camp.nextstep.edu.missionutils.Randoms`의 `pickNumberInRange()`를 활용한다.
   - 사용자가 입력하는 값은 `camp.nextstep.edu.missionutils.Console`의 `readLine()`을 활용한다.
- 프로그램 구현을 완료했을 때 `src/test/java` 디렉터리의 `ApplicationTest`에 있는 모든 테스트 케이스가 성공해야 한다. **테스트가 실패할 경우 0점 처리한다.**

<br>

---


## 📝 License

This project is [MIT](https://github.com/woowacourse/java-racingcar-precourse/blob/master/LICENSE) licensed.
