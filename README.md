## EARLY WORD

직장인들을 위한 단어공부 웹 어플리케이션

### 취지
- 영어 공부 시작하는게 너무 비싸다... 구독제인데 기본 10000원이 넘어감.
- 우리는 싼 가격에 기능도 최소화해서 내겠다는 취지

### 경쟁 업체
- 매일 11시 (https://everyday11.kr/)
- 말해보카, 산타 토익 등

### 타겟
- 직장인, 출퇴근 길에 !간단한 공부!를 원하는 사람들

### 기능
- 매일 아침 7시에 카카오톡으로 10개씩 단어 보내기
- 10개 단어 중 몇 개 랜덤으로 뽑아서 문제 내주기 (카카오톡으로 단어와 함께 문제 푸는 페이지 주소 공유)
- 단어는 카테고리 별로 설정할 수 있음. (토익 beginner, intermediate, advanced)
- 단어 및 문제는 AI가 생성한다.


### 주요 제한 사항
- 비즈니스 로직... 단어나 문제를 미리 생성해서 넣어 두어야 할 거 같은데 데이터 관리는 어떻게 할 수 있나? 
    어떻게 하느냐에 따라 DB 성능이 천지 차이일듯 싶다
- 카카오에 의존적이다. (어쩔 수 없을듯..)
- 매일 같은 시간에 보내다 보니 동시성 문제도 고려해야 할 거 같다.

### 예상 이점
- 서비스 크기를 잘 맞추면 실제로 배포해볼 수 있다. 당장 나만해도 쓸만할 듯
- 확장에 열려있다. 핵심 기능은 단어 생성해서 보내주는 것만 해도 되지만, 
통계적인 부분이나 쿠폰, 포인트 제도 등을 도입하면 서비스할 수 있는 기능들을 많이 넣을 수 있다.
- DB나 쿼리문에 대해 공부해 볼 수 있다.