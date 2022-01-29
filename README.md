# React Native Introduction

## 📎 Nomad coder link

- [왕초보를 위한 React Native 101 - weather](https://nomadcoders.co/react-native-for-beginners)

---

## 📝 강의 요약

- 세팅
  - node.js 버전 14.7 이상으로
- node.js 업데이트 방법
  - mac
    - ` npm cache clean -f`
    - `npm install -g n`
    - `n stable`
  - windows
    - stable 버전 node.js 다시 다운받기
- Expo 준비단계
  - `npm install --global expo-cli` 입력
  - 핸드폰으로 expo 앱 다운 후 로그인  
    (Expo or Expo go)
- React Native

  - 브라우저가 아님
  - 아름다운 번역기
  - 인터페이스로 운영체제 사이에 존재함
  - 작동법
    1.  native(ios, 안드로이드)에 event가 기록됨  
        즉 ios와 안드로이드가 터치 이벤트를 감지
    2.  ios와 안드로이드는 이벤트에 대한 데이터를 수집함
    3.  react native는 그 정보를 가지고 JSON 메시지를 생성
    4.  Javascript 즉 우리의 코드는 그 메시지를 받음
    5.  Javascript에서 코드 실행(UI 변경 등)
    6.  react native 는 native 운영체제에게 메시지를 보냄  
        5번에서 실행될 코드에 대해서 말함
    7.  UI가 업데이트 됨

- 시작하기
  - cmd에 `expo init 앱이름` 입력 후 enter 누르기
  - cmd에서 expo login으로 로그인
  - npm start
