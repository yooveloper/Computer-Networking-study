q1. 301 status code의 용도, 301과 302의 차이는 ?

- 301 영구적인 리다이렉트 , 302 일시적인 리다이렉트

q2. 쿠키의 단점을 말해주시고 대체제를 말씀해주세요

- 보안 이슈
- 서버단에서는 세션으로 관리
- 인메모리 저장소나 DB에서 세션관리
- 세션 클러스터링
- JWT
- 브라우저에서 제공하는 localstorage / sessionstorage

q3. 캐시는 서버이면서 클라이언트라는 표현이 나오는데 어떤 이유 때문일까요?

q4. DNS 서버에서 해당 IP주소를 찾지 못할 경우 어떻게 될까요?

- DNS_PROBE_FINISHED_NXDOMAIN

q5. DNS_PROBE_FINISHED_NXDOMAIN 와 HTTP status 404의 차이점은?

- 전자는 DNS 에러, 후자는 서버에 요청 리소스가 없을때 응답

HTTP 메서드의 멱등성이 무엇인가요?

HTTP 메서드 중 PUT과 PATCH를 비교해 주세요.

- PUT은 다 덮어씌움, PATCH는 부분만 변경

DNS가 무엇인가요? 언제 사용하나요?

데이터 센터가 뭘까?

TCP와 UDP 차이 그리고 TCP/IP

르윈의 TCP UDP

HTTP 쿠키와 세션이란?

웹 캐시(WEB Cache)란 무엇인가?(특징)

단순 전자우편 전송 프로토콜(SMTP)이란?

SMTP를 알아보자

DNS & CDN

소켓 프로그래밍

UDP 소켓 프로그래밍

소켓 프로그래밍(TCP, UDP)

(면접) 서비스를 Stateless하게 설계하면 어떤 장점과 단점이 있을까요?

- 수평적 규모 확장에 유리

- 인증 복잡도 증가

Transport Protocol 이 제공하는 서비스의 분류 기준에는 어떤것들이 있을까요?

-

TCP와 UDP의 차이에 대해서 설명해주세요

UDP를 사용해볼만한 애플리케이션에는 어떤것들이 있을까요?

- 스트리밍 서비스

(면접) 3-way handshake는 어떤식으로 이루어지나요?

(면접) 4-way handshake는 어떤식으로 이루어지나요?

HTTP 요청 메세지의 첫번째 줄에는 어떤것들이 들어가나요?

- method, url, http version

Connection 헤더의 역할이 뭔가요?

Last-Modified 헤더의 역할이 뭔가요?

- 캐시에 이용

(면접) HTTP 상태코드의 번호대 별 차이에 대해 알고있는지

- 500, 503 status code 차이점

- 500 : runtime exception

- 503 : DDOS 등으로 인한 과부하

(면접) HTTP 상태코드 301과 302의 차이가 뭔가요?

(면접) HTTP 상태코드 401과 403의 차이가 뭔가요?

- 401 : 인증 실패, 403 : 권한 없음

쿠키가 뭔가요?

쿠키가 어떤식으로 작동하는지 설명해주세요

- 디스크에 저장 -> 내 컴퓨터 저장소

웹 캐싱에 대해서 설명해주세요

웹 캐싱을 사용해서 얻는 이점이 뭔가요?

웹 캐싱을 사용해서 문제가 발생할 수 있는 경우에는 어떤게 있을까요?

- 원본 데이터 불일치

HOL Blocking이 뭔가요?

HTTP 1.1 버전과 2.0 버전의 차이점에 대해서 설명해주세요

DNS가 뭔가요?

DNS의 부하분산(DNS 라운드 로빈)이 뭔가요?

DNS의 계층구조는 어떻게 되어있나요?

(면접) 인터넷창에 www.google.com을 쳤을때 사용자 호스트와 구글 서버 간에 어떤 일들이 일어나는지 네트워크 관점에서 설명해주세요

DNS 레코드가 뭔가요?

DNS 레코드 튜플의 Type이 CNAME이라면 Name과 Value에는 어떤값이 들어가나요?

DNS 메세지는 뭔가요?

프로세스는 서로 어떻게 통신할까요?

서버에서 여러 프로그램들이 동작할 때 클라이언트는 어떻게 특정 프로그램으로 접속할 수 있을까요?

http : 80
https: 443

80 으로 443 리다이렉트 -> SSL 인증서가 있으면 -> 웹서버 설정에서 리다이렉트 -> nginx, apache든 웹서버가 없으면? -> 요청이 거부가 된다

API란 무엇인가요?

UDP, TCP의 차이점에 대해서 설명해주세요.

대칭키, 공개키에 대해서 설명해주세요.

HTTP에 대해서 설명해주세요.

왜 http는 tcp를 사용할까요?

- 데이터의 손실을 방지하기 위해서

http는 왜 무상태 프로토콜일까요?

http 상태코드에 대해서 설명해주세요.

http는 무상태 프로토콜인데, 상태는 어떻게 저장해야 할까요?

응답 시간을 줄이기 위해 어떤 방법들이 있을까요?

- 클라이언트 <-> 서버 간에 CDN

DNS는 무엇이고 어떻게 동작할까요?
