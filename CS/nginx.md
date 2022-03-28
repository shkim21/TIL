- Nginx(웹서버)
    - 동시접속 처리에 특화된 웹 서버 프로그램. 가볍고 성능 좋은 엔진
    1. 웹 서버(http server) 역할 : http 프로토콜 이용해서 HTML, CSS, Javascript, 이미지 같은 정보 웹 브라우저에 전송
        1. HTTP 프로토콜 : TCP/IP 통신 위에서 동작, 기본 포트 80
            1. TCP/IP : 두 개의 프로토콜 사용하여 데이터 통신 하는 것
                1. IP(internet protocol): 복잡한 네트워크 망 패킷통신(데이터 작은 조각들로 나뉘어서 보냄)
                2. TCP(transmission control protocol) : 조각난 데이터 받으면서 순서 안 맞으면 정렬, 누락된 데이터 점검하여 다시 요청
    2. 리버스 프록시 : 배후 서버로부터 데이터 가져옴 (로드 밸런서) (클라 요청과 서버 응답 중개)
        1. 요청에 버퍼링 있기 때문
        2. 요청 배분
        3. 비동기 처리 방식(또 다른 작업 처리 가능) ↔ 동기 처리 : 하나의 요청에 하나의 작업
    - event-driven 구조 - 한개, 고정된 프로세스만 생성하여 사용, 비동식 방식 요청들 concurrency하게 처리가능
    - 구조 : 하나의 master process, 다수의 worker process
        - master process : 설정파일 읽고, 유효성 검사, worker process 관리
        - worker process : 모든 요청 처리