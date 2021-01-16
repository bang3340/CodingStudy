# Flutter tutorial

### The Flutter tutorials teach you how to use the Flutter framework to build mobile applications for iOS and Android.

Choose from the following:


레이아웃 구축
Flutter의 레이아웃 메커니즘을 사용하여 레이아웃을 구축하는 방법. 기본 원칙을 배웠 으면 샘플 스크린 샷을위한 레이아웃을 빌드합니다.
Flutter 앱에 상호 작용 추가
아이콘을 탭할 수 있도록 "Flutter에서 레이아웃 만들기"에서 만든 간단한 레이아웃 앱을 확장합니다. 위젯의 상태를 관리하는 다양한 방법에 대해서도 설명합니다.
Flutter의 애니메이션
Flutter 애니메이션 패키지 (컨트롤러, 애니메이션 가능, 커브, 리스너, 빌더)의 기본 클래스를 설명하며 애니메이션 API의 다양한 측면을 사용하여 트윈 애니메이션 진행을 안내합니다.
Flutter 앱 국제화
Flutter 애플리케이션을 국제화하는 방법을 알아보세요. 앱에서 사용자의 언어 및 형식 지정WIn 규칙을 사용하여 콘텐츠를 표시 할 수 있도록하는 위젯 및 클래스에 대한 가이드입니다.


## FLUTTER WINDOWS 설치 

https://flutter.dev/docs/get-started/install/windows

시스템 요구 사항
Flutter를 설치하고 실행하려면 개발 환경이 다음과 같은 최소 요구 사항을 충족해야합니다.

운영 체제 : Windows 7 SP1 이상 (64 비트), x86-64 기반
디스크 공간 : 1.32GB (IDE / 도구 용 디스크 공간은 포함되지 않음).
도구 : Flutter는 환경에서 사용할 수있는 이러한 도구에 의존합니다.
Windows PowerShell 5.0 이상 (Windows 10에 사전 설치됨)
Windows 명령 프롬프트에서 Git 사용 옵션 이있는 Windows 2.x 용 Git .

Windows 용 Git이 이미 설치된 git경우 명령 프롬프트 또는 PowerShell에서 명령을 실행할 수 있는지 확인 합니다.

Flutter SDK 받기
Flutter SDK의 안정적인 최신 릴리스를 받으려면 다음 설치 번들을 다운로드하십시오.


다른 릴리스 채널 및 이전 빌드는 SDK 릴리스 페이지를 참조하세요.

zip 파일을 추출하고 flutter Flutter SDK의 원하는 설치 위치 (예 :)에 포함합니다 C:\src\flutter.

 경고 :C:\Program Files\ 상승 된 권한이 필요한 디렉토리에 Flutter를 설치하지 마십시오 .

설치 번들의 고정 버전을 설치하지 않으려면 1 단계와 2 단계를 건너 뛸 수 있습니다. 대신 GitHub 의 Flutter 리포지토리 에서 소스 코드를 가져와 필요에 따라 브랜치 또는 태그를 변경합니다. 예를 들면 :

content_copy
C:\src>git clone https://github.com/flutter/flutter.git -b stable
이제 Flutter 콘솔에서 Flutter 명령을 실행할 준비가되었습니다.

경로 업데이트
일반 Windows 콘솔에서 Flutter 명령을 실행하려면 다음 단계를 수행하여 PATH환경 변수에 Flutter를 추가하세요 .

시작 검색 창에서 'env'를 입력하고 계정에 대한 환경 변수 수정을 선택 합니다 .
사용자 변수 에서 경로 라는 항목이 있는지 확인합니다 .
항목이 있으면 기존 값의 구분 기호 로 flutter\bin사용에 전체 경로를 추가하십시오 ;.
항목이 없으면 Path전체 경로를 flutter\bin값으로 사용하여 이름이 지정된 새 사용자 변수를 만듭니다 .
이러한 변경 사항을 적용하려면 기존 콘솔 창을 닫았다가 다시 열어야합니다.

 참고 : Flutter의 1.19.0 dev 릴리스부터 Flutter SDK에는 dart명령과 함께 명령이 포함되어있어 flutter Dart 명령 줄 프로그램을보다 쉽게 ​​실행할 수 있습니다. Flutter SDK를 다운로드하면 호환되는 Dart 버전도 다운로드되지만 Dart SDK를 별도로 다운로드 한 dart경우 두 버전이 호환되지 않을 수 있으므로 Flutter 버전이 경로에서 첫 번째 인지 확인 하세요. 다음 명령 (macOS, Linux 및 chrome OS에서)은 flutter및 dart명령이 동일한 bin디렉토리 에서 시작되어 호환 되는지 여부를 알려줍니다 . (일부 Windows 버전은 유사한 where명령을 지원합니다 .)

content_copy
 which flutter dart
  /path-to-flutter-sdk/bin/flutter
  /usr/local/bin/dart
위에 표시된 것처럼 두 명령은 동일한 bin디렉토리 에서 제공되지 않습니다 . /path-to-flutter-sdk/bin이전 명령 /usr/local/bin(이 경우)의 명령 을 사용하도록 경로를 업데이트하십시오 . 변경 사항이 적용되도록 셸을 업데이트 한 후 which또는 where명령을 다시 실행 하면 flutter및 dart명령이 이제 동일한 디렉토리에서 온 것으로 표시되어야합니다 .

content_copy
 which flutter dart
  /path-to-flutter-sdk/bin/flutter
  /path-to-flutter-sdk/bin/dart
dart명령 에 대해 자세히 알아 보려면 dart -h 명령 줄에서 실행 하거나 dart 도구 페이지를 참조하세요.

운영 flutter doctor
경로에 Flutter 디렉토리가있는 콘솔 창 (위 참조)에서 다음 명령을 실행하여 설정을 완료하는 데 필요한 플랫폼 종속성이 있는지 확인합니다.

content_copy
C:\src\flutter>flutter doctor
이 명령은 환경을 확인하고 Flutter 설치 상태에 대한 보고서를 표시합니다. 설치해야 할 다른 소프트웨어 나 수행 할 추가 작업에 대한 출력을주의 깊게 확인하십시오 ( 굵은 텍스트로 표시됨).

예를 들면 :

content_copy
[-] Android 툴체인-Android 기기 용 개발
    • D : \ Android \ sdk의 Android SDK
    ✗ Android SDK에 명령 줄 도구가 없습니다. https://goo.gl/XxQghQ에서 다운로드
    • Android SDK를 다시 설치하거나 업데이트하십시오.
      자세한 지침은 https://flutter.dev/setup/#android-setup을 방문하십시오.
다음 섹션에서는 이러한 작업을 수행하고 설정 프로세스를 완료하는 방법에 대해 설명합니다. 누락 된 종속성을 설치 한 후에는 flutter doctor명령을 다시 실행하여 모든 것이 올바르게 설정되었는지 확인할 수 있습니다.

 참고 : 경우 flutter doctor플러터 플러그인 또는 두 다트는 안드로이드 스튜디오의 플러그인 수익률이 설치되지 않은,로 이동 편집기 설정이 이 문제를 해결합니다.

 경고 : 이 flutter도구는 Google 애널리틱스를 사용하여 기능 사용 통계 및 기본 오류 보고서 를 익명으로보고 합니다 . 이 데이터는 시간이 지남에 따라 Flutter 도구를 개선하는 데 사용됩니다.

Flutter 도구 분석은 첫 실행시 전송되지 않습니다. 보고를 비활성화하려면을 입력 flutter config --no-analytics합니다. 현재 설정을 표시하려면을 입력하십시오 flutter config. 분석을 옵트 아웃하면 옵트 아웃 이벤트가 전송되고 Flutter 도구에서 추가 정보를 보내지 않습니다.

Flutter SDK를 다운로드하면 Google 서비스 약관에 동의하는 것입니다. 참고 : Google 개인 정보 취급 방침 은이 서비스에서 데이터가 처리되는 방식을 설명합니다.

또한 Flutter에는 사용 메트릭과 충돌 보고서를 Google에 보낼 수있는 Dart SDK가 포함되어 있습니다.

Android 설정
 참고 : Flutter는 Android 플랫폼 종속성을 제공하기 위해 Android Studio의 전체 설치에 의존합니다. 그러나 여러 편집기에서 Flutter 앱을 작성할 수 있습니다. 이후 단계에서 이에 대해 설명합니다.

Android Studio 설치
Android Studio를 다운로드하여 설치 합니다.
Android Studio를 시작하고 'Android Studio 설정 마법사'를 진행합니다. 그러면 Flutter에서 Android 용으로 개발할 때 필요한 최신 Android SDK, Android SDK 명령 줄 도구 및 Android SDK 빌드 도구가 설치됩니다.
Android 기기 설정
Android 기기에서 Flutter 앱을 실행하고 테스트 할 준비를하려면 Android 4.1 (API 레벨 16) 이상을 실행하는 Android 기기가 필요합니다.

장치에서 개발자 옵션 및 USB 디버깅 을 활성화 합니다. 자세한 지침은 Android 문서 에서 확인할 수 있습니다 .
Windows 전용 : Google USB 드라이버를 설치합니다 .
USB 케이블을 사용하여 휴대폰을 컴퓨터에 연결합니다. 장치에 메시지가 표시되면 장치에 액세스 할 수 있도록 컴퓨터를 인증합니다.
터미널에서 flutter devices명령을 실행하여 Flutter가 연결된 Android 기기를 인식하는지 확인합니다. 기본적으로 Flutter는 adb 도구의 기반이 되는 Android SDK 버전을 사용합니다 . Flutter가 다른 Android SDK 설치를 사용하도록하려면 ANDROID_SDK_ROOT환경 변수를 해당 설치 디렉터리로 설정해야합니다 .
Android 에뮬레이터 설정
Android 에뮬레이터에서 Flutter 앱을 실행하고 테스트 할 준비를하려면 다음 단계를 따르세요.

머신에서 VM 가속 을 활성화 합니다.
Android Studio를 실행 하고 AVD Manager 아이콘을 클릭 한 다음 Create Virtual Device…를 선택합니다 .
이전 버전의 Android Studio에서는 대신 Android Studio> Tools> Android> AVD Manager를 실행 하고 Create Virtual Device…를 선택해야 합니다. ( Android 하위 메뉴는 Android 프로젝트 내부에서만 표시됩니다.)
프로젝트가 열려 있지 않은 경우 구성> AVD 관리자 를 선택하고 가상 장치 생성…을 선택할 수 있습니다 .
장치 정의를 선택하고 다음을 선택 합니다.
에뮬레이트하려는 Android 버전에 대한 시스템 이미지를 하나 이상 선택하고 다음을 선택 합니다. 86 또는 x86_64의 이미지가 좋습니다.
Emulated Performance에서 Hardware-GLES 2.0 을 선택 하여 하드웨어 가속 을 활성화 합니다 .
AVD 구성이 올바른지 확인하고 Finish를 선택 합니다 .

위 단계에 대한 자세한 내용은 AVD 관리를 참조하세요 .

Android Virtual Device Manager 의 도구 모음에서 실행 을 클릭 합니다. 에뮬레이터가 시작되고 선택한 OS 버전 및 장치에 대한 기본 캔버스가 표시됩니다.
웹 설정
Flutter는 Flutter beta채널을 사용하여 웹 애플리케이션을 구축하기위한 초기 지원을 제공합니다 . 웹 개발에 대한 지원을 추가하려면 위의 설정을 완료 한 후 다음 안내를 따르세요 .

