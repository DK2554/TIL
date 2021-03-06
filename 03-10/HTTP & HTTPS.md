# HTTP 

- HTTP(Hyper Text Transfer Protocol)
 - 서버/클라이언트 모델을 따라 데이터를 주고 받기 위한 프로토콜
 - 구조
    - HTTP는 애플리케이션 레벨의 프로토콜 TCP/IP 위에서 작동한다.
        - Method,Path,Version,Headers,Body등으로 구성
        - but http는 암호화가 되지 않은 평문 데이터 전송하는 프로토콜이였기 때문 제3자가 정보를 조회 할 수 있다,
        그래서 등장한것이 HTTPS

- HTTPS(Hyper Text Transfer Protocol Secure)
    - HTTP에 데이터 암호화가 추가된 프로토콜
    - 네트워크 상에서 중간에 제3자가 정보를 볼 수 없도록 공개키 암호화를 지원
    
    - 공개키/개인키
        - HTTPS는 공개키/개인키 암호화 방식을 이용해 데이터를 암호화
        - 공개키와 개인키는 서로를 위한 1쌍의 키이다.
        - 공개키: 모두에게 공개가능한 키
        - 개인키: 나만 가지고 알고 있어야 하는 키

    - 공개키와 개인키로 암호화 효과
        - 공개키 암호화: 공개키로 암호화 하면 개인키로만 복호화 할 수 있다-> 개인키는 나만 가지고 있으므로 나만 볼 수 있음
        - 개인키 암호화 : 개인키로 암호화 하면 공개키로만 복호화 할 수 있음 -> 공개키는 모두에게 공개되어 있으므로 내가 인증한 정보임을 알려 신뢰성 보장



[ HTTPS의 동작 과정 ]
HTTPS는 SSL과 같은 프로토콜을 사용하여 공개키/개인키 기반으로 데이터를 암호화하고 있다. 데이터는 암호화되어 전송되기 때문에 임의의 사용자가 데이터를 조회하여도 원본의 데이터를 보는 것은 불가능하다.

그렇다면 이제 서버는 클라이언트가 요청을 보낼 때 암호화를 하기 위한 공개키를 생성해야 하는데, 일반적으로는 인증된 기관(Certificate Authority) 에 공개키를 전송하여 인증서를 발급받고 있다. 자세한 과정은 다음과 같다.

A기업은 HTTP 기반의 애플리케이션에 HTTPS를 적용하기 위해 공개키/개인키를 발급함

CA 기업에게 돈을 지불하고, 공개키를 저장하는 인증서의 발급을 요청함

CA 기업은 CA기업의 이름, 서버의 공개키, 서버의 정보 등을 기반으로 인증서를 생성하고, CA 기업의 개인키로 암호화하여 A기업에게 이를 제공함

A기업은 클라이언트에게 암호화된 인증서를 제공함

브라우저는 CA기업의 공개키를 미리 다운받아 갖고 있어, 암호화된 인증서를 복호화함

암호화된 인증서를 복호화하여 얻은 A기업의 공개키로 데이터를 암호화하여 요청을 전송함



[참고](https://mangkyu.tistory.com/98?category=762469)