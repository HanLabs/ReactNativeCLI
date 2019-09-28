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
```
```
expo init AwesomeProject
```
```
cd AwesomeProject
npm start # you can also use: expo start
```

신기하게도, `$ expo init {PROJECT}` 를 실행하면 CLI 를 통해 여러 옵션을 선택할 수 있고 이것이 반영된 예제 프로젝트가 생성된다.
Xcode 와 같은 툴이 없어도 시뮬에서 실행이 가능하고, node console 에서 QR 코드를 통해 디바이스에서 실행도 가능하다.

### 2) React Native CLI Quickstart
모바일 개발툴과 함께 RN 을 개발할 수 있는 일반적인 방법.

아래 명령어들을 순서대로 실행한다. 이 때 발견된 문제는 없었다.

```
brew install yarn
brew install node
brew install watchman
brew tap AdoptOpenJDK/openjdk
brew cask install adoptopenjdk8
```
```
pm install -g react-native-cli
```
```
XCode > Preferences > Location > Command Line Tools(DropBox) > 가장 최신 버전으로 선택 & 설치
```
```
react-native init ReactNativeCLI
```
> 위 명령어의 결과 `command not found: react-native` 에러가 발생하였다. <br>
> `$ export PATH=$HOME/.nodenv/versions/10.10.0/bin:$PATH` 을 입력한 후
> `$ npx react-native init ReactNativeCLI` 처럼 npx 를 사용해 init 에 성공할 수 있다.


```
cd ReactNativeCLI && react-native run-ios
```
명령으로 앱이 정상 실행되는것을 확인할 수 있다. (위 스핏의 결과와 동일한 에러가 발생한다면 npx 를 붙여서 run) <br>
이전 Realm 가이드 시도와는 달리 Error 없이 앱이 실행되었다 (감동 ^_ㅠ..)
