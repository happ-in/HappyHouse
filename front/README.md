<img src = "https://i.imgur.com/pTP5x2C.png" width = "300px"><br>

## 개요
* SPA(Single Page Application) 을 지향하고, 컴포넌트 기반 설계. 
* NPM기반 dependencies 관리
* Axios를 통해 비동기 방식으로 HTTP 데이터 요청 (ajax)
## 프로젝트 구성

### Components
<img src = "https://i.imgur.com/cS3m3DV.png" width = "600px">

### Main page
<img src = "https://i.imgur.com/sA7hlhW.png" width = "600px">

### Dependencies
| module | version | 사용 이유 |
| -------- | -------- | -------- |
| vue     | 2.6.12   | -     |
| axios     | 0.21.1     | HTTP Request 모듈 |
| chart.js     | 2.9.4     | 코로나 확진자 수 차트 시각화 |
| vue-router     | 3.2.0     | 라우팅 기능 구현     |
| vuetify     | 2.4.0     | UI toolkit     |
| vuex     | 3.4.0     | 상태 관리     |
| vuex-persistedstate     | 4.0.0-beta.3     | vuex store 초기화 방지 |

## Discussion
* 페이지 이동시나 새로고침하는 경우가 발생하게 되는데 이럴 때 지금까지 vuex의 store에 가지고 있거나 계산되어져 있던 모든 값들이 초기화 되어버리는 상황 발생
    * vuex-persistedstate 모듈을 통하여 초기화 방지


