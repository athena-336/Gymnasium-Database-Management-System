# Gymnasium Management System | 體育館資料庫管理系統

A comprehensive management information system for school gymnasiums, integrating venue tracking and equipment rental. The system features a robust relational database design to streamline physical processes and improve facility accessibility for both students and administrators.
「酷酷的體育館資料庫管理系統」整合了場地查看與器材租借功能，透過完善的關連式資料庫設計，將繁瑣的實體行政流程數位化，提升體育館使用的便利性與管理效率。

> **國立政治大學 資料庫管理課程 · NCCU DBMS Final Project · 2022 · 第九組**

---

## 🎯 Objective | 分析目標
To eliminate unnecessary physical paperwork and improve gymnasium utility. The system allows students to check venue availability (to avoid peak hours) and enables administrators to manage inventory and rental records efficiently.
去除不必要的實體流程，增加體育館使用便利性。使用者可預先查看場地剩餘空間以避開尖峰時段，管理者則能有效率地管控器材庫存與租借紀錄。

---

## 🛠 Pipeline | 處理流程
1. **Requirement Analysis:** Identifying functional needs for two user roles (User & Manager). / 需求分析：定義使用者與管理者的功能需求。
2. **Conceptual Design:** Developing Entity-Relationship Diagrams (ERD) to map complex relationships. / 概念設計：繪製實體關係圖（ERD）以規劃資料關聯。
3. **Logical Design:** Converting ERD to a Relational Model with primary/foreign key constraints. / 邏輯設計：將 ERD 轉換為關連式模型，設定主鍵與外來鍵約束。
4. **Data Dictionary:** Defining detailed metadata for users, equipment, and venue records. / 資料字典：定義使用者、器材與場地紀錄的詳細資料格式。
5. **Operational Implementation:** Ensuring referential integrity and multi-user concurrency control. / 實作規劃：確保參照完整性與多使用者併發控制（一次僅限一人修改）。

---

## 💻 Tech Stack | 技術棧
* **Database:** Relational Database Model (SQL-based logic)
* **Design Tools:** ERD Modeling, Relational Schema Design
* **Documentation:** Functional Dependency Diagrams (FDD)
* **Core Concepts:** Entity/Referential Constraints, Normalization

---

## 🧠 System Features | 系統功能
* **Venue Tracking (場地查看):** Real-time status of courts, gym occupancy, and weekly schedules (no login required for browsing). / 即時查看各場地每週使用狀況與健身房人數。
* **Equipment Rental (器材租借):** Authenticated users can request and manage equipment rentals online. / 使用者登入後可直接在平台上租借器材。
* **Admin Dashboard (管理者介面):** Tools for inventory management, rental history tracking, and penalty (illegal record) management. / 管理者可管控庫存、更新場地狀態並管理違規紀錄。

---

## 📊 Logical Design | 邏輯設計
* **Entities:** USER, MANAGER, EQUIPMENT, VENUE, RENT_RECORD.
* **Constraints:** Primary keys (UserID, EquipID) ensure uniqueness; Referential constraints prevent data loss during deletions (e.g., maintaining audit trails for alumni).
* **Integrity:** Implemented operational constraints to handle graduation data cleanup and multi-manager access.

---

## 👥 Team Members | 團隊成員
* **黃筠茜 (Athena Huang):** Database Design & Requirement Analysis / 資料庫設計與需求分析
* **鄭筑云:** Project Coordination / 專案協調
* **李慈琳:** Logical Design / 邏輯設計
* **江翊瑄:** Requirement Analysis / 需求分析
* **莊詠婷:** Implementation Planning / 實作規劃

---

## 中文簡介
本專案為政大資料庫管理課程之期末作品。系統分為「場地」與「器材」兩大面向，並針對學生（使用者）與體育館管理員提供不同權限。學生可透過系統查看即時場地使用率（如健身房人數）與租借器材；管理員則可進行庫存管控、租借歷史查詢與違規紀錄管理。專案涵蓋完整資料庫開發流程：從 ERD 繪製、正規化分析、到關連式模型建立，並嚴格遵循實體與參照完整性限制。
