# Favorly - 線上商品收藏與推薦系統 🎯

> 一個基於 Spring Boot 開發的 RESTful API 專案，實作商品收藏與推薦功能，支援 JWT 認證、模組化設計與 DDD 架構，適合作為學習與履歷展示專案。

---

## 📌 專案簡介

Favorly 提供使用者瀏覽商品、收藏喜愛項目，並根據收藏紀錄推薦相似商品。後台支援管理員新增商品、檢視熱門收藏統計，並以清晰模組區分各功能，完整實踐 Spring Boot 架構開發流程。

---

## 🧱 系統模組結構

| 模組名稱 | 功能說明 |
|----------|----------|
| `User`     | 使用者註冊、登入、個人資料管理 |
| `Auth`     | JWT 登入與驗證流程 |
| `Product`  | 商品瀏覽、分類查詢、關鍵字搜尋 |
| `Favorite` | 收藏商品、多對多關聯、個人推薦清單 |
| `Admin`    | 商品上架/下架、收藏數統計、權限控管 |

---

## 🔧 技術選型

| 類別       | 技術說明                        |
|------------|---------------------------------|
| 語言       | Java 21                         |
| 框架       | Spring Boot 3.x                |
| ORM        | Spring Data JPA + Hibernate    |
| 認證授權   | Spring Security + JWT          |
| 資料庫     | MySQL 8.x                      |
| 文件生成   | Springdoc OpenAPI (Swagger UI) |
| 測試       | JUnit 5 + MockMvc              |
| 建構工具   | Maven                           |
| 架構風格   | 模組化 + 分層架構（DDD導向）     |

---

## 🚀 專案功能亮點

- ✅ RESTful API 設計
- ✅ JWT 登入與授權保護
- ✅ 多對多關聯（使用者 ↔ 商品收藏）
- ✅ 商品分類與模糊搜尋
- ✅ 基於收藏紀錄推薦商品（簡易推薦邏輯）
- ✅ 管理者權限驗證與統計 API
- ✅ DTO/Entity 分離與統一錯誤處理
- ✅ Swagger API 文件生成

---

## 📁 專案目錄結構（模組化範本）

```bash
src/
└── main/
    └── java/
        └── com/example/favorlybackend/
            ├── modules/
            │   ├── user/
            │   │   ├── controller/
            │   │   ├── service/
            │   │   ├── domain/
            │   │   │   ├── entity/
            │   │   │   └── repository/
            │   │   ├── dto/
            │   │   └── exception/
            │   └── ...
            ├── config/
            └── FavorlyBackendApplication.java
```

---

## 🛠️ 開發環境建議

* JDK 21
* **MySQL 8.x**
* IntelliJ IDEA / VS Code
* Postman / Swagger UI 測試 API

---

## 📚 學習重點與實踐面向

* 清楚理解 Spring Boot 的三層架構（Controller, Service, Repository）
* 熟悉 RESTful API 設計原則
* 學習 Spring Security 與 JWT 實作
* 掌握 JPA Entity 設計與關聯關係
* 實踐模組化與 Domain 分離架構（符合業界實務）

