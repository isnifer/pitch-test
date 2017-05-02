---

# E2E Tips & Tricks

---

# С чего начать?

---

### tipsi-appium-helper

---

1. Конфигурируемый модуль для запуска тестов
2. Использует Appium как платформу для тестов
3. Написан на JS
4. Test-runner и ассерты - tape
5. Можно подключить другой runner
6. Режим playground
7. Максимально полные логи

---

```sh
npm i tipsi-appium-helper -g

# or

npm i tipsi-appium-helper --save-dev
```

---

Yarn, покойся с миром

---

#### Конфигурация - RC file (.appiumhelperrc)

---

```json
{
  "testsGlob": "./__tests__/e2e/suites",
  "register": "./__tests__/e2e/setup",
  "fullReset": true,
  "ios": {
    "appPath": "./ios/build/Build/Products/Release-iphonesimulator/tipsi.app"
  },
  "android": {
    "appPath": "./android/app/build/outputs/apk/app-release.apk"
  }
}
```
---
