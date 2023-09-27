# 2023-2-BE-STUDY-2주차 과제

## HTTP(Hypertext Transfer Protocol)
TCP/IP 기반 이동통신규약.

### 특징
#### Transfer layer
TCP/IP 기반으로 서버-클라이언트 간 요청과 응답을 전송함
*TCP: 인터넷 상에서 데이터를 메세지의 형태로 보내기 위해 IP와 함께 사용되는 프로토콜. 패킷(데이터 블록)을 추적 및 관리한다. IP의 신뢰성 문제 보완.
#### 비연결성
클라이언트가 서버와 한 번 연결을 맺은 후 클라이언트의 요청에 대해 서버가 응답을 마치면 연결을 끊는다.
#### 무상태성
비연결성으로 인해 서버가 두 요청 간 어떠한 데이터도 유지하지 않는다. 이러한 이유로 서버는 클라이언트를 식별하지 못한다.

### 연결 과정
1. TCP 연결을 열어준다.
2. 클라이언트가 HTTP 메시지를 전송한다.
3. 서버가 보낸 응답을 읽는다.
4. TCP 연결을 닫거나 다른 요청을 위해 재사용한다.

### HTTP Message: request <-> response
HTTP 메시지의 구조

Method /(경로) http 버전

헤더

#### HTTP Message 의 Method
1. 주로 사용하는 메소드
GET(리소스 조회)

POST(요청 데이터 처리 ex.등록)->멱등하지 않다

PUT(리소스 대체 혹은 해당 리소스 생성)

PATCH(리소스 부분 변경)->멱등하지 않다

DELETE(리소스 삭제)

2. 이외 메소드
HEAD(GET과 동일하지만 상태줄과 헤더만을 반환)
OPTIONS(리소스에 대한 통신 가능 옵션을 설명) CONNECT(서버 터널 설정) TRACE(리소스 경로를 따라 루프백 테스트 수행)

#### 상태 코드
1. 1xx(Informational): 요청 수신 및 처리 중
2. 2xx(Successful): 요청 정상 처리
3. 3xx(Redirection): 요청 완료를 위한 추가 행동 필요
4. 4xx(Client Error): 클라이언트 오류
5. 5xx(Server Error): 서버 오류


## HTTP VS HTTPS

HTTPS는 HTTP를 추가로 암호화 하기 위해 SSL/TLS 인증서를 사용한다.
웹 사이트에 대한 권위, 신뢰성 및 검색 엔진 순위 개선이 용이하다는 장점이 있다. 

## 아래 API에 대해 RESTful URI 설계 
1. 이벤트 목록 조회
GET /events
2. 이벤트 조회
GET /events/{eventid}
3. 이벤트 등록
POST /events
4. 이벤트 수정
PATCH /events/{eventid}
5. 이벤트 삭제
DELETE /events/{eventid}
6. 이벤트 상태 변경
PATCH /events/{eventid}/status
8. 특정 이벤트의 주문 목록 조회
GET /events/{eventid}/orders
8. 멤버 목록 조회
GET /members/
9. 특정 멤버 권한 변경
PATCH /members/{memberid}/authority
10. 특정 멤버 정보 조회
GET /members/{memberid}
11. 특정 멤버 정보 변경
PATCH /members/{memberid}
12. 멤버 등록
POST /members