# TIL

"build": "GENERATE_SOURCEMAP=false react-scripts build"


2020.12

### react-native-cli
react-native info

#### issue1: react-native not found
환경변수설정 export PATH="blahblah/blahblah/bin:$PATH"
package.json에 yarn path로 script 추가 해두었음

#### issue2: brew를 사용하여 jdk 인스톨 실패
android studio 설치 시 포함
웹사이트에서 다운로드

#### issue3: react-native-webview
cd ios => pod install

#### issue4: error adb: command not found
brew install android-platform-tools
https://richwind.co.kr/58

#### issue5: 환경변수 설정
ls -l -a ~/.bash_profile
touch -c ~/.bash_profile
open -e ~/.bash_profile

export ANDROID_HOME=$HOME/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools

source ~/.bash_profile

안드로이드 스튜디오 sdk manager에서 설치
Android 9(Pie)
Android SDK Platform 28
Intel x86 Atom_64 System Image
Google APIs Intel x86 Atom_64 System Image


#### issue6: error Failed to install the app
1. /android/gradle/wrapper/gradle-wrapper.properties 에서 6.3 버전으로 변경
2. /android/local.properties 생성 후 sdk.dir = /Users/<USERNAME>/Library/Android/sdk
