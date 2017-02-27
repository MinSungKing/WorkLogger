# 출근했는지 로그를 남기자!

## 버전히스토리
  - 0.1.4
    - Apple Macbook은 Padding을 통해서 60Bytes Packet으로 보냄
    - struct unpack 버그 수정
  - 0.1.3
    - 출근한 사람이 없을 경우 기록하지 않음
  - 0.1.2
    - 출근한 인원 Set 형식으로 출력
    - 잠자는 시간을 위해 ini 템플릿 수정
    - 대문자로 등록된 MAC 소문자로 변환
  - 0.1.1
    - 잠자는 시간 설정파일로 조정 가능
  - 0.1.0
    - 초기버전 완성

## 사용법
  1. .ini파일을 세팅한다.
  2. 관리자 권한으로 실행한다.
  3. alive.csv 파일로 출력이 된다.


## 목표
  - 시각화
  - 잠자는 시간 설정파일로 조정(0.1.1 패치)
  - 출근한 인원 Set 형식으로 출력(0.1.2 패치)
    - False Negative를 줄이기 위해 여러 MAC Address 등록할 수 있도록 위함
  - 대문자로 등록된 MAC을 소문자로 변환(0.1.2 패치)
  - 출근한 사람이 없을 경우 출력하지 않음(0.1.3 패치)
  - 개인 출근 내역 익스포트 기능
    - 개인 인증 서비스가 있어야 함
  - 출력 파일 이름을 설정 파일에서 확인
  - 소켓 자는 시간 설정 파일에서 확인
  - 출력 파일 csv 헤더 추가
  - Wireless interface를 활용해 Probe Request 메시지를 탐색
    - AP에 연결하지 않고도 확인 가능
