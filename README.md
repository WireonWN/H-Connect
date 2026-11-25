<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/wordmark-dark.png" />
    <source media="(prefers-color-scheme: light)" srcset="assets/wordmark-light.png" />
    <img src="assets/wordmark-light.png" alt="Horizon Connect" width="640" />
  </picture>
</p>

# Horizon Connect 1.0.0 для macOS

🙀 Завёз первый выпуск Horizon Connect для Mac

💻 Apple Silicon · macOS 15+

[![Скачать DMG для macOS](assets/download-macos-dmg.svg)](https://github.com/WireonWN/H-Connect/releases/download/macos-v1.0.0/HorizonConnect-1.0.0-macOS-arm64.dmg) · [Установка](INSTALL.md#macos)

## Что есть в первой версии

- Импорт подписок и конфигов по ссылке, из файла и по QR
- Карточки подписок с датой окончания и остатком времени
- Поиск серверов, сортировка по пингу и проверка всей подписки
- Выбор приложений, которые подключаются напрямую
- Стеклянные меню, светлая и тёмная темы, настройка шрифта и масштаба

## Немного техники

- Интерфейс на Qt, сетевая часть AirX на Rust
- Прозрачный прокси через системное расширение Apple Network Extension
- DMG для arm64 подписан Developer ID и нотариализован Apple

## Установка

1. Откройте DMG и перетащите Horizon Connect в «Программы»
2. Запустите приложение и добавьте подписку или конфиг
3. При первом подключении разрешите сетевое расширение, если macOS покажет запрос

Если что-то пошло не так, укажите версию macOS и шаги до ошибки

[Сообщить об ошибке](https://github.com/WireonWN/H-Connect/issues/new/choose)

[Сборки для остальных платформ](https://github.com/WireonWN/H-Connect/tree/main#загрузка)
