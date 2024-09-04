# Server Wallet SDK

Server Wallet SDK Repository에 오신 것을 환영합니다. <br>이 Repository는 서버 월렛을 개발하기 위한 SDK를 제공합니다.

## 폴더 구조
```
did-wallet-sdk-server
├── CHANGELOG.md
├── CLA.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE.dependencies.md
├── MAINTAINERS.md
├── README_ko.md
├── README.md
├── RELEASE-PROCESS.md
├── SECURITY.md
├── docs
│   └── api
│        ├── WALLET_SDK_SERVER_API.md
│        ├── WALLET_SDK_SERVER_API_ko.md
│        └── WalletSDKError.md
└── source
    └── did-wallet-sdk-server
        ├── .gitignore
        ├── build.gradle
        ├── gradle
        │    └── wrapper
        ├── gradlew
        ├── gradlew.bat
        ├── libs
        │    └── did-crypto-sdk-server-1.0.0.jar 
        ├── README_ko.md
        ├── README.md
        ├── settings.gradle
        └── src
```

|  이름 |         역할                    |
| ------- | ------------------------------------ |
| source  |  SDK 소스코드 프로젝트             |
| docs  |   문서            |
| ┖ api  |  API 가이드 문서          |
| ┖ design |  설계 문서            |
| sample  |  샘플 및 데이터            |
| README.md  |  프로젝트의 전체적인 개요 설명     |
| CLA.md             | Contributor License Agreement|
| CHANGELOG.md| 프로젝트 버전별 변경사항           |
| CODE_OF_CONDUCT.md| 기여자의 행동강령            |
| CONTRIBUTING.md| 기여 절차 및 방법           |
| LICENSE.dependencies.md| 프로젝트 의존성 라이브러리에 대한 라이선스  |
| MAINTAINERS.md          | 유지관리 가이드      |
| RELEASE-PROCESS.md      | 릴리즈 절차       |
| SECURITY.md| 보안취약점 보고 및 보안정책  | 

## 라이브러리

1. 서버 프로젝트에 `did-crypto-sdk-server-1.0.0.jar` 파일을 복사한다.
2. 서버 프로젝트의 build gradle에 아래 의존성을 추가한다.

```groovy
    implementation files('libs/did-crypto-sdk-server-1.0.0.jar')

    implementation 'org.bouncycastle:bcprov-jdk18on:1.78.1'
    implementation 'com.google.guava:guava:33.2.1-jre'
    implementation 'com.google.code.gson:gson:2.8.9'
    implementation 'org.slf4j:slf4j-api:2.0.7'
```
3. `Gradle`을 동기화하여 의존성이 제대로 추가되었는지 확인한다.

## API 참조

API 참조는 [여기](docs/api/WALLET_SDK_SERVER_API_ko.md)에서 확인할 수 있습니다.

## 기여

Contributing 및 pull request 제출 절차에 대한 자세한 내용은 [CONTRIBUTING.md](CONTRIBUTING.md)와 [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) 를 참조하세요.

## 라이선스
Copyright 2024 Raonsecure