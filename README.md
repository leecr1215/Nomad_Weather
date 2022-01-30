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
- react native의 rule
  - div 대신 View 태그 사용
  - 존재하는 텍스트는 모두 text component 안에 들어가야 함
- `StyleSheet.create`
  - object를 생성하는데 사용
  - 사용하는 이유
    - 좋은 자동 완성 기능을 제공함
    - component 정리에 좋음
- Layout System
  - `<View>`는 display: flex가 기본 값
  - 웹의 flex direction의 기본값은 row지만 모바일은 column임
- ScrollView
  - 내부의 component와 View를 자식으로 담을 수 있고 화면의 스크롤을 사용할 때 사용하는 component
  - 스크롤 방향은 horizontal을 통해 가로 또는 세로로 변경 가능
  - `contentContainerStyle={{styles.변수}}`
  - `pagingEnabled`로 페이지처럼 만들 수 있음
  - `showsHorizontalScrollIndicator={false}` 로 스크롤 바를 없앨 수 있음
  - `indicatorStyle="white"`으로 스크롤바의 색상을 변경할 수 있음(ios에서만 작용)
  - 자세한 사용방법 : [reactnative.dev](https://reactnative.dev/docs/scrollview)
- Dimensions
  - 화면 크기를 얻는 API
- location
  - `expo install expo-location` 입력
  - `Location.requestForegroundPermissionAsync()`으로 유저에게 위치 접근 권한 동의 알림창 보여줌
  - `Location.getCurrrentPositionAsync()`으로 user의 위도와 경도를 알아냄
  - `Location.reverseGeocodeAsync()`으로 위도와 경도를 이용해 주소를 가져옴
  - openweatherorg의 api를 이용해 날씨를 가져옴
- toFixed()
  - 원하는 소수점만큼 남길 수 있음
  - (12.12).toFixed(1) -> 12.1
- expo/vector-icons
  - icons.expo.fyi 사이트에 가면 아이콘 확인 가능
