# vivo PC Suite (vivo Office Kit) — CN Adapted for macOS (Apple Silicon)

Полностью адаптированная китайская версия **vivo PC Suite v7.0.6 (arm64)** для macOS (Apple Silicon): сохранены все расширенные функции китайской сборки при полностью локализованном интерфейсе на русском и английском языках.

Fully adapted Chinese edition of **vivo PC Suite v7.0.6 (arm64)** for macOS (Apple Silicon): keeps all extended CN features with full Russian & English localization.

---

## Что изменено / Key Changes

- **Все функции CN-версии сохранены (`IS_EXPORT: false`, `SaleArea=CN`)**: резервное копирование (`VivoBackup`), Календарь, Диктофон с ИИ-расшифровкой, XiaoV AI, ретрансляция уведомлений/SMS, облачные сервисы и аккаунт CN.
- **Поддержка любых смартфонов vivo / iQOO**: снята региональная блокировка по `ro.vivo.product.overseas` — подключаются как китайские (OriginOS CN), так и глобальные устройства.
- **Полная локализация RU + EN**:
  - Дополнены словари `ru_RU` и `en_US` до 100% соответствия ключам `zh_CN` (включая раздел «Диктофон»).
  - Локализованы все захардкоженные китайские строки интерфейса в CN-модулях, HTML-окнах, системных разрешениях `Info.plist`, меню Finder и расширении виртуальной камеры.
  - Добавлены все системные `.lproj`-локализации из глобальной версии для `pcsuite.app` и `vcontrol.app`.
  - Включён переключатель языка в **Настройки → Общие → Язык** и автоматическое определение системного языка macOS (включая региональные локали вроде `ru_KZ` → `ru_RU`).
  - Локализован встроенный модуль удалённого управления (`vcontrol.app`).

---

## Скачивание и установка / Download & Install

Скачайте установщик **`pcsuite_v7.0.6-arm64-cn-adapted.pkg`** из раздела **[Releases](../../releases/latest)**.

- **Версия / Version:** `7.0.6` (macOS 10.13+, Apple Silicon / `arm64`)
- **SHA-256:** `48947e82ff14c611a0c6e00c507f3939176ef53d9821da986915aecca99f1dbd`

### Установка (macOS Gatekeeper)

Поскольку пакет пересобран локально и не заверен Apple Notary:

1. Нажмите правой кнопкой мыши по `pcsuite_v7.0.6-arm64-cn-adapted.pkg` → **«Открыть»** (или установите через терминал):
   ```bash
   sudo installer -pkg pcsuite_v7.0.6-arm64-cn-adapted.pkg -target /
   ```
2. При первом запуске `/Applications/pcsuite.app` macOS может ~5–10 секунд проверять подпись, после чего приложение откроется на языке системы. Переключить язык в любой момент можно в **Настройки → Общие → Язык**.

---

## Примечание / Disclaimer

Неофициальная модификация оригинального пакета vivo PC Suite v7.0.6 для личного использования. Все права на оригинальное ПО принадлежат vivo Mobile Communication Co., Ltd.
