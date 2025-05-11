.local-plugins内に、flutter unity view widget の android 324 向けに直したブランチを持ってきてください。

これの、build.gradle のうちcompileSdkVersion を 33 にして、targetSdkVersion を 34 にしてsplashScreenの警告が出ないようにする必要があります。

クリーンビルドのコマンド

```bash
cd /Users/a-kun/uaal_flutter_324/android && ./gradlew clean && cd .. && fvm flutter clean && fvm flutter pub get && fvm flutter build apk --release
```