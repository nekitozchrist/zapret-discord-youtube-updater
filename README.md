<p align="center">
<h1 align="center">
  🚀 Скрипт автоматического обновления 🚀
<h1 align="center">
  zapret-discord-youtube
</h1></p>
  
### 📦 Назначение

Скрипты для бесшовного обновления уже установленной версии [zapret-discord-youtube](https://github.com/flowseal/zapret-discord-youtube).
Скачайте новую версию, распакуйте содержимое в папку `update` внутри основного каталога и запустите `update.bat`.

### ✨ Что делает update.bat

- Проверяет, что папка `update` не пустая и всё на месте.
- Если zapret запущен как служба — останавливает, а после обновления перезапускает с той же стратегией.
- Переносит новую версию поверх старой, сохраняя ваши списки и настройки.
- После завершения очищает папку `update`.

### 🛠 Что делает warp_masque.bat

Отдельный скрипт для перевода Cloudflare WARP на протокол **MASQUE**.

### ⚙️ Требования

- **ОС:** Windows 10/11
- **Права администратора** — обязательны (скрипт запросит сам)
- **Основная программа:** установленный [zapret-discord-youtube](https://github.com/flowseal/zapret-discord-youtube/releases)
- [**Cloudflare WARP**](https://developers.cloudflare.com/cloudflare-one/team-and-resources/devices/cloudflare-one-client/download) — опционально, только для `warp_masque.bat` (лежит в релизе с апдэйтэром)
- **PowerShell 5.1+** (есть из коробки в Windows 10/11)

### 📥 Использование

1. Распакуйте [скрипт обновления](https://github.com/nekitozchrist/zapret-discord-youtube-updater/releases/download/1.0.0/ZDY_Updater_v1.0.0.zip) в корень установленного zapret-discord-youtube.
2. Новую версию [zapret-discord-youtube](https://github.com/flowseal/zapret-discord-youtube/releases) распакуйте в папку `update`.
3. Запустите `update.bat`.

### 📁 Состав

| Файл | Назначение |
|------|------------|
| `update.bat` | Главный скрипт обновления |
| `update_core.bat` | Служебный скрипт управления сервисом |
| `update_script.ps1` | PowerShell-скрипт обновления файлов |
| `warp_masque.bat` | Скрипт настройки WARP MASQUE |
| `update/` | Папка для размещения новой версии |
