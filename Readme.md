# 📦 OptiOffice iOS SDK

Swift SDK для интеграции с **OptiOffice API**.  
Сгенерирован автоматически из [OpenAPI спецификации](https://github.com/llkenny/optioffice-contracts).

---

## 🚀 Возможности
- Типобезопасные модели (DTO) на Swift.  
- Удобный `APIClient` для работы с эндпоинтами (`/auth/login`, `/orgs`, `/spaces`, …).  
- Поддержка async/await.  
- Совместим с iOS 15+ и Swift 5.7+.  

---

## 📲 Установка

### Swift Package Manager (SPM)

В Xcode:  
`File → Add Packages → https://github.com/llkenny/optioffice-ios-sdk.git`

Или в `Package.swift`:
```swift
dependencies: [
    .package(url: "https://github.com/llkenny/optioffice-ios-sdk.git", exact: "1.0.0")
]
```

## 🛠 Использование
```swift
import OptiOfficeSDK

let client = APIClient(baseURL: URL(string: "https://api.example.com")!)

// Логин
let tokens = try await client.auth.login(LoginRequest(email: "user@example.com", password: "secret"))

// Получить список организаций
let orgs = try await client.orgs.list()
print(orgs.items)
```

## 📦 Версионирование
- SDK версионируется по SemVer.
- Ломающие изменения → новый major (2.0.0).
- Минорные изменения (новые поля, эндпоинты) → minor (1.1.0).
- Исправления → patch (1.0.1).

## ⚠️ Важно
- DK не содержит секретов и токенов.
- URL API и токены аутентификации должны передаваться приложением.
- Для конфигурации используйте .env или параметры сборки.
