# 모든 개발자를 위한 HTTP 웹 기본 지식

## TCP & UDP

### TCP

- 인터넷 프로토콜 스택 4계층

- 애플리케이션 계층 HTTP,FTP

- 전송 계층 TCP,UDP

- 인터넷 계층 IP

- 네트워크 인터페이스 계층

+ TCP 특징

- 연결지향
- 데이터 전달 보증
- 순서 보장

- 신뢰할 수 있는 프로토콜

- 대부분TCP 사용

+ UDP 특징

- 연결지향 
- 데이터 전달 보증x
- 순서 보장x
- 데이터 전달 및 순서가 보장되지 않지만 단순하고 빠름


============================

# HTTP 특징

    - 클라이언트 서버 구조

    - 무상태 프로토콜, 비연결성

    - HTTP 메세지

    - 단순함, 확장 가능


## 클라이언트 서버 구조

     - Request , Response 구조

     - 클라이언트는 서버에 요청 보내고, 응답이 올때까지 대기

     - 서버가 요청에 대한 결과를 만들어서 응답

## 무상태 프로토콜 Stateless 

    - 서버가 클라이언트의 상태를 보존X

    - 장점: 서버 확장성 높음

    - 단점: 클라이언트가 추가 데이터 전송 
