# XSS (Cross Site Scripting)

- Xss는 웹 어플리케이션에 악의적으로 스크립트를 삽입해서 공격하는 기법.

- 만약 웬 어플리케이션에서 데이터를 서버로 저장할 때 데이터를 검증하지 않거나 XSS에 대한 방어 대비가 없다면 스크립트가 포함된 데이터가 저장되어 유저로 하여금 원치 않는 스크립트를 실행시킬 수 있다.
- 이러한 방식의 위험성은 일반적으로 자바스크립에서 발생하지만 VB스크립트,Active X등과 같은 동적 데이터를 생성하는 모든 언어에서 발생 할 수 있다. 이는 유저의 정보를 탈취하거나, 조직 내부의 데이터가 탈취되는 등 매우 위험한 상황으로 이어 질 수 있음
 이에 대비해 네이버에서 개발한 XSS 필터링 기법인 luch-xss-servlet-filter

 

[사용법](https://hailey0.tistory.com/39)








출처: https://shxrecord.tistory.com/212 [첫 발]
