[![Dart](https://img.shields.io/badge/Dart-0175C2?logo=dart&logoColor=white)](https://pub.dev/packages/fancy_text_reveal)  ![Flutter](https://img.shields.io/badge/Flutter-02569B?logo=flutter&logoColor=white)
[![Test](https://github.com/Shadow60539/club_penguin_game/actions/workflows/test.yml/badge.svg?style=flat&logo=appveyor)](https://github.com/Shadow60539/club_penguin_game/actions/workflows/test.yml)

# Club Penguin 

원본소스 : https://github.com/Shadow60539/club_penguin_game

오픈소스 클럽펭귄 빌드, 커스터마이징 프로젝트.

빌드시 firebase RDBMS와 연동. auth 활성화 해야함
google-services.json 파일을 아래의 폴더경로에 복붙
1. [PROJECT]\app\
2. [PROJECT]\app\src\
3. [PROJECT]\app\src\debug\

TCP 통신이라 실시간으로 왔다갔다 통신하거나 부드럽지는 않지만
상대방의 대략적인 위치는 기록됨.(움직일때 상대방 끊김현상은 있으나 채팅에는 문제없음)

펭귄의 실시간 위치를 갱신하려면 UDP 소켓서버를 고려해야할듯

TODO : 
1. 그룹채팅방을 만들어 들어가게하기
2. 그룹채팅별 채팅 로그


아래는 원본 소스코드 제작자의 README.md
클럽 펭귄을 소개하고 있음


![lib](images/poster.png)

[![Playstore](images/google-play-badge.png)](https://play.google.com/store/apps/details?id=com.nonamelight.penguin_chat_game)

### Introduction 🚀

> Club Penguin
A multiplayer game involving penguins and anonymous chat in a virtual 2D world

Before we start, you can take a look at the app:

![Output sample](images/demo.gif)




### Usage 🎨

To clone and run this application, you'll need [git](https://git-scm.com) and [flutter](https://flutter.dev/docs/get-started/install) installed on your computer. From your command line:

```bash
# Clone this repository
$ git clone https://github.com/Shadow60539/social_media_game.git

# Go into the repository
$ cd social_media_game.git

# Install dependencies
$ flutter packages get

# Run the app
$ flutter run
```


### Packages 📦


Some very good packages are used in this project.



Package | Description
---|---
[flame](https://pub.flutter-io.cn/packages/flame) | A minimalistic Flutter game engine
[firebase_auth](https://pub.flutter-io.cn/packages/firebase_auth) | Firebase Authentication
[firebase_core](https://pub.flutter-io.cn/packages/firebase_core) | To use the Firebase Core API
[firebase_database](https://pub.flutter-io.cn/packages/firebase_database) | Firebase Realtime Database 
[dartz](https://pub.flutter-io.cn/packages/dartz) | Support functional programming in Dart
[build_runner](https://pub.flutter-io.cn/packages/build_runner) | Build Custom Models
[flutter_bloc](https://pub.flutter-io.cn/packages/flutter_bloc) | BLoC State Management
[flutter_launcher_icons](https://pub.flutter-io.cn/packages/flutter_launcher_icons) | Replace launcher icon
[freezed](https://pub.flutter-io.cn/packages/freezed) | Code generation for immutable classes
[google_fonts](https://pub.flutter-io.cn/packages/google_fonts) | Support google fonts
[injectable](https://pub.flutter-io.cn/packages/injectable) | Dependency injection
[lint](https://pub.flutter-io.cn/packages/lint) | Rules handler for Dart
[lottie](https://pub.flutter-io.cn/packages/lottie) | Lottie files animations
[mockito](https://pub.flutter-io.cn/packages/mockito) | Mock library for Dart
[provider](https://pub.flutter-io.cn/packages/provider) | Provider State Management

### Directory Structure 🏢

The project directory structure is as follows:

```
├── android
├── asset
├── build
├── images
├── ios
├── lib
├── test
├── analysis_options.yaml
├── pubspec.lock
├── pubspec.yaml

```

![lib](images/lib.png)



Directory | Description
---|---
application | State management layer
core | Core files which depend on all these layers
domain | Model and contract layer
infrastructure | Data layer
presentation | Widget layer
