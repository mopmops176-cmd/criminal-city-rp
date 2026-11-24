CRIMINAL CITY RP — ANDROID PROJECT

Это проект Android-приложения, который упаковывает текущую рабочую игру в полноэкранное приложение WebView.
Игра запускается как приложение, а не отдельной вкладкой Chrome. Для загрузки Three.js из CDN и внешних ресурсов нужен интернет.

КАК СОБРАТЬ APK:
1. Установить Android Studio на компьютер.
2. Открыть в Android Studio папку CriminalCityAndroid.
3. Дождаться синхронизации Gradle.
4. Выбрать Build -> Build Bundle(s) / APK(s) -> Build APK(s).
5. APK появится в app/build/outputs/apk/debug/app-debug.apk.
6. Перенести APK на телефон и установить, разрешив установку приложений из этого источника.

ВАЖНО:
- В этом окружении нет Android SDK/Gradle, поэтому готовый APK здесь собрать и проверить нельзя.
- Онлайн-вход, зависящий от среды claude.use('room'), не становится публичным сервером от упаковки в APK. Для настоящего онлайна нужен отдельно размещённый backend и адаптация клиента.
- Это Android-оболочка текущей рабочей версии, а не перенос на нативный 3D-движок уровня GTA San Andreas.

ЕСЛИ У ВАС ТОЛЬКО ТЕЛЕФОН:
Смотрите PHONE_BUILD_RU.txt. В проект добавлен GitHub Actions workflow .github/workflows/build-apk.yml, который собирает APK в облаке без Android Studio.
