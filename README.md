# 📱 Mobile QA Test Assignment — iOS Application (Stage Beta)

## 👤 Candidate Information
* **Name:** Андрій Діброва
* **Role:** Junior Mobile QA Engineer
* **Target OS:** iOS (Apple iPhone 17 / iOS 26.5.2)

---

## 📌 Executive Summary
Даний репозиторій містить публічний звіт про проведене функціональне, UI/UX, локалізаційне та офлайн-тестування (Airplane Mode) тестової збірки мобільного застосунку **Elomia (Stage Beta)**. 

За результатами випробувань було виявлено та задокументовано **13 підтверджених дефектів** (включаючи закладені критичні пастки безпеки, UI Collapse та блокування навігації).

> 🏆 **Project Achievement:** Звіт посів місце в **ТОП-кандидатах** за результатами перевірки серед 160+ виконаних тестових завдань (із 800+ загальних відгуків).

---

## 🛠 Test Environment Specifications
| Parameter | Value / Characteristic |
| :--- | :--- |
| **Device Model** | Apple iPhone 17 |
| **Operating System** | iOS 26.5.2 (Beta / Stage build) |
| **Display** | Super Retina XDR OLED, 120Hz (ProMotion), Dynamic Island |
| **Hardware** | Apple A19 / 8 GB RAM |
| **System Language** | Ukrainian |
| **Network Conditions** | Wi-Fi 6E / 5G / Airplane Mode (Offline) |

---

## 📋 Bug Summary Table

| # | Bug Title | Severity | Module / Screen | Summary Description |
| :-: | :--- | :-: | :--- | :--- |
| **1** | Disconnected emergency line `0 800 100 102` | **Critical** | SOS / Help | Calling "Лінія безкоштовної психологічної допомоги" fails with operator error "Service disconnected". |
| **2** | Out-of-service helpline `0 800 501 701` | **Critical** | SOS / Help | Calling "Лінія кризової підтримки" connects to an out-of-service automated message. |
| **3** | Global UI Collapse: Screen content permanently disappears on fast scroll | **Critical** | Systemic (Profile, Settings, Practices, Chat) | Entire content turns blank (black screen) after fast scroll and does NOT return; requires full app restart. |
| **4** | Systemic carousel disappearance on upward flick/swipe | **High** | Systemic ("Для вас", "Практики") | Horizontal icon/filter carousels fly off-screen and permanently disappear when dragged upwards. |
| **5** | Exercise freezing in SOS ("Знайдіть свій якір") | **High** | SOS / Help | Interactive practice text freezes and audio fails to play on first launch until app restart. |
| **6** | Exercise freezing in "Практики" section | **High** | Practices | Interactive exercises freeze on launch (text stuck, no voice), requiring app restart. |
| **7** | Practice titles and descriptions in English | **Medium** | Practices | All titles and descriptions for specific practices remain in English fallback, while app UI is Ukrainian. |
| **8** | Entire Lectures sub-section falls back to English | **Medium** | Practices / Lectures | No Ukrainian localization present across the entire content module for Lectures. |
| **9** | Onboarding carousel freezes on Notification screen | **Medium** | Onboarding | Preview cards/carousel indicators (`...`) freeze and fail to respond to swipe gestures. |
| **10** | Small tap target area for chat text input field | **Medium** | Main Chat | Tapping outer bounds of the input container fails to trigger focus/keyboard; requires tap on placeholder text. |
| **11** | UI freezing/lag when switching "Для вас" tabs | **Low** | For You | Noticeable delay/lag (approx. 1s) when switching category filters (Поради, Афірмації, Мотивація). |
| **12** | Audio latency when changing voice in practice | **Low** | Practices / Settings | Changing the guide voice during active exercise causes noticeable audio latency/lag. |
| **13** | Onboarding flow freeze on "Продовжити" in Airplane Mode despite offline status notification | **High** | Systemic / Offline Handling / Onboarding | Tapping "Продовжити" during offline onboarding causes indefinite UI freeze instead of disabling the button or blocking progress. |

---

## 📎 Documentation & Attachments
* Оригінальний файл звіту з повним описом та скріншотами: [`тестове завдання_Діброва_Андрій.docx`](./тестове%20завдання_Діброва_Андрій.docx)
