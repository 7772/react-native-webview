# react-native-webview #v6.2.2-intent

**0. package.json 의 dependencies 를 모두 설치할 때** 

```
  $ yarn install
```

**1. react-native-webview 만 설치할 때**

```
  $ yarn add https://github.com/7772/react-native-webview\#v6.2.2-intent
```

**2. `react-native run-android`**

**3. ./lib/WebView Error 발생**

> react-native-webview 가 typescript 로 만들어져있기 때문에 .ts 파일을 .js 파일로 컴파일하는 과정을 추가해야함

**4. `cd node_modules/react-native-webview && yarn && npm run build && cd ../..`**

**5. `react-native run-android`**

**6. jest-hash-map Error 발생**

> react-native-webview 파일 내 node_modules 에 포함된 react-native 파일과 본 프로젝트의 react-native 파일 간 충돌이 발생, 따라서 lib 내 파일을 지워준다.

**7. `rm -rf node_modules/react-native-webview/node_modules/react-native/`**

**8. `react-native run-android`**