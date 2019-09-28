# ReactNativeCLI by HanSJin

[Realm RN Starter](https://academy.realm.io/kr/posts/react-native/) 예제를 버리고 [RN-Getting Started](http://facebook.github.io/react-native/docs/getting-started) 예제로 변경

> Realm RN Starter 예제는 이 곳에서 확인 > [HanLabs/ReactNative](https://github.com/HanLabs/ReactNative)

## References for RN
https://academy.realm.io/kr/posts/react-native/

### What's the defference between `React`, `Ractive`, and `ReactNative`?

* [React](https://facebook.github.io/react/) 는 페이스북이 웹 개발을 쉽게 하기 위해 만든 기술. <br>
커스텀 컴포넌트를 만들고 쉽게 조합해서 뷰를 손쉽게 만들 수 있습니다.
* **Reactive** 는 마이크로소프트가 창안한 개념으로 스트림과 비동기 처리등을 LINQ에 영향을 받은 방법으로 깔끔하게 처리할 있게 한 패러다임. <br>
예를 들어 [RxJava](https://github.com/ReactiveX/RxJava), [RxAndroid](https://github.com/ReactiveX/RxAndroid), [ReactiveCocoa](https://github.com/ReactiveCocoa/ReactiveCocoa) 등등 ..
* [React Native](https://facebook.github.io/react-native/) 는 리액트의 접근 방법을 모바일로 확장하는 페이스북의 오픈소스 프로젝트.

## Getting Started

RN 예제 프로젝트의 종류는 아래 2가지 나뉜다.

### 1) Expo CLI Quickstart
Expo 는 XCode, Android Studio 같은 모바일 개발 툴 없이 모바일 개발을 진행할 수 있다.

```
npm install -g expo-cli

expo init AwesomeProject

cd AwesomeProject
npm start # you can also use: expo start
```

신기하게도, `$ expo init {PROJECT}` 를 실행하면 CLI 를 통해 여러 옵션을 선택할 수 있고 이것이 반영된 예제 프로젝트가 생성된다.
