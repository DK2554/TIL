# XSS (Cross Site Scripting)

- Xss는 웹 어플리케이션에 악의적으로 스크립트를 삽입해서 공격하는 기법.

- 웹 애플리케이션에서 일어나는 취약점으로 관리자가 아닌 권한이 없는 사용자가 웹 사이트에 스크립트를 삽입하는 공격 기법

- 만약 웬 어플리케이션에서 데이터를 서버로 저장할 때 데이터를 검증하지 않거나 XSS에 대한 방어 대비가 없다면 스크립트가 포함된 데이터가 저장되어 유저로 하여금 원치 않는 스크립트를 실행시킬 수 있다.
- 이러한 방식의 위험성은 일반적으로 자바스크립에서 발생하지만 VB스크립트,Active X등과 같은 동적 데이터를 생성하는 모든 언어에서 발생 할 수 있다. 이는 유저의 정보를 탈취하거나, 조직 내부의 데이터가 탈취되는 등 매우 위험한 상황으로 이어 질 수 있음
 이에 대비해 네이버에서 개발한 XSS 필터링 기법인 luch-xss-servlet-filter

 

[사용법](https://hailey0.tistory.com/39)

## 공격 종류 및 방법

1. Persistent XSS 
 - 지속형 xss 공격 
 - 지속적으로 피해를 입히는 XSS공격이다 데이터베이스에 저장이되어 Stored XSS 공격이라고 부르기도 한다.

2. Reflected Xss 
 - 반사형 XSS 공격
 - 사용자에게 입력 받은 값을 서버에 되돌려 주는 곳에서 발생한다.
 - 사용자에게 입력 받은 검색어를 그대로 보여주는 곳이나 사용자가 입력한 값을 에러 메세지에 포함하여 보여주는 곳에 악성스크립트가 삽입되면, 서버가 사용자의 입력값을 포함해 응답해 줄 때 스크립트가 실행된다.
3. DOM based XSS
 - DOM based XSS는 악의적인 스크립트가 포함된 URL을 사용자가 요청하게 되어 브라우저를 해석하는 단계에 발생하는 공격이다 




[참고](https://noirstar.tistory.com/266)
[첫 발]https://shxrecord.tistory.com/212 
