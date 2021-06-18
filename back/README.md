<img src = "https://i.imgur.com/pTP5x2C.png" width = "300px"><br>

## 개요
* 웹 프로젝트에 필요한 DB 스키마 제작
* Spring Boot를 사용하여 웹 프로젝트에 필요한 Rest API를 제작
* 외부 API 서버프로그래밍을 통한 호출

## 프로젝트 구성
<img src="https://i.imgur.com/k2A2fdT.png" width="500px">

## DB 스키마 
<img src="https://i.imgur.com/kiRXaTs.png" width="800px">

## Dependencies   

|dependency|용도|
|-|-|
|spring-boot-starter|의존성과 설정을 자동화해주는 모듈|
|mybatis|Java-SQL 사이의 자동 매핑을 지원하는 ORM 프레임워크|
|Lombok|Getter/Setter 등 메소드를 Annotation으로 대체|
|mysql-connector-java|mysql과 연결|



## Discussion
* 네이버 뉴스 검색 API 사용 시에 **CORS 발생**
    * 웹 브라우저에서 실행했던 API를 서버프로그래밍으로 옮겨와 작성하여 해결

* 아파트 정보를 가져올 때, 데이터가 많이 불러와서 시간이 오래 소요
    *  join문이 cross join으로 데이터가 많아짐. join 조건과 left join으로 변경
