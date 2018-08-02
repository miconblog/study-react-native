# React Native

## Expo 와 함께 Eject 하기

개발 초기엔 Expo 를 이용해 폰에 올려서 보기 편하기 때문에 일단은 Expo를 유지한채 [Eject][1] 해봅니다. 
CRNA 를 탈출하면 직접 빌드를 해야하므로 react-native-cli 도 필요합니다. 

```bash
$> npm i -g react-native-cli
```

이제 탈출해봅시다! ExpoKit을 선택합니다.

```bash
$> npm run eject

? How would you like to eject from create-react-native-app?
  React Native: I'd like a regular React Native project.
❯ ExpoKit: I'll create or log in with an Expo account to use React Native and the Expo SDK.
  Cancel: I'll continue with my current project structure.

```

Expo 계정이 필요하므로 이미 있는 경우엔 기존 계정을 이용합니다. 

```bash
An Expo account is required to proceed.

? How would you like to authenticate?
  Make a new Expo account
❯ Log in with an existing Expo account
  Cancel
```

iOS 앱을 만들려면 [앱을 구분하는 식별자][2]를 지정해야 합니다. 

- Uniform Type Identifier(UTI): alphanumeric characters (A-Z,a-z,0-9), hyphen (-), and period (.)
- 보통 reverse DNS 노테이션을 사용합니다. (ex. com.myCompany.myApp) 


[Android 앱 식별자][3]도 필요합니다. 


[1]:https://github.com/react-community/create-react-native-app/blob/master/EJECTING.md
[2]:https://stackoverflow.com/questions/11347470/what-does-bundle-identifier-mean-in-the-ios-project
[3]:https://stackoverflow.com/questions/6273892/android-package-name-convention
