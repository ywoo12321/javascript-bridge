# 기능 구현 구상

## **_1. 다리 함수_**

- [x] **생성 함수**
  - [x] 입력 받은 다리길이에 해당하는 리스트를 생성하고 '0' or '1' 중 랜덤한 숫자를 저장한다
  - [x] upBridge 와 downBridge를 생성한다.
  - [x] 랜덤 리스트를 가지고 reduce를 통해 Bridge의 형태를 만든다.

## **_2. 다리 건너기 함수_**

- [x] **U, D 입력 받기 함수**
  - [x] U, D를 각 1, 0 으로 바꿔서 정답 비교 함수에 추가
  - [x] 해당 위치 답안과 일치 한다면
    - [x] 해당 다리에 'O' 추가, 밑 다리에 ' ' 추가
    - [x] U, D 입력 받기 함수 실행
  - [x] 해당 위치 답안과 일치 하지 않다면
    - [x] 해당 다리에 'X' 추가, 밑 다리에 ' ' 추가
    - [x] 재시작 여부 함수 실행
- [x] **정답 비교 함수**
  - 랜덤 리스트와 비교해서 U를 입력했을 시 '1' D를 입력했을 시 '0'으로 비교하여 해당 인덱스 값과 일치하는지 확인
- [x] **재시작 함수**
  - [x] R, Q입력 받게 실행
    - [x] R을 입력 받았을 시
      - count += 1
      - U, D 입력 받기 함수 실행
    - [x] Q를 입력 받았을 시
      - 현재 상태를 보여준다.
      - Console.close()
