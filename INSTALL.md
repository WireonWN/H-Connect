[Horizon Connect](README.md) / Установка

# Загрузка и установка

## Загрузка

| Система | Сборки | Инструкция |
| :--- | :--- | :--- |
| Android | [![APK](assets/badge-apk.svg)](https://github.com/WireonWN/H-Connect/releases/download/android-v2.4.0/HorizonConnect-2.4.0-Android.apk) [![Google Play](assets/badge-play.svg)](https://play.google.com/store/apps/details?id=com.horizon.connect) | [Android](#android) |
| Windows | [![Windows .exe](assets/download-windows-exe.svg)](https://github.com/WireonWN/H-Connect/releases/download/windows-v2.2.0/HorizonConnect-2.2.0-Windows-x64-Setup.exe) | [Windows](#windows) |
| macOS | [![macOS .dmg](assets/download-macos-dmg.svg)](https://github.com/WireonWN/H-Connect/releases/download/macos-v1.0.0/HorizonConnect-1.0.0-macOS-arm64.dmg) | [macOS](#macos) |
| Linux | [![Debian / Ubuntu .deb](assets/download-linux-deb.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v2.2.0/HorizonConnect-2.2.0-Linux-amd64.deb) <br /> [![Fedora .rpm](assets/download-linux-rpm.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v2.2.0/HorizonConnect-2.2.0-Linux-x86_64.rpm) <br /> [![Arch / Manjaro .pkg.tar.zst](assets/download-linux-arch.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v2.2.0/HorizonConnect-2.2.0-Linux-x86_64.pkg.tar.zst) <br /> [![Linux .zip](assets/download-linux-zip.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v2.2.0/HorizonConnect-2.2.0-Linux-x86_64.zip) | [Linux](#linux) |

Файлы конкретной версии находятся в **Assets** её релиза

## Android

[Скачать APK 2.4.0](https://github.com/WireonWN/H-Connect/releases/download/android-v2.4.0/HorizonConnect-2.4.0-Android.apk) или установить через [Google Play](https://play.google.com/store/apps/details?id=com.horizon.connect)

Откройте APK на устройстве и разрешите установку из выбранного источника, если Android попросит
Требуется Android 8.0 или новее
Для обновления установленной копии должны совпадать подписи и подходить код версии; используйте тот же источник установки

## Windows

[Скачать установщик 2.2.0](https://github.com/WireonWN/H-Connect/releases/download/windows-v2.2.0/HorizonConnect-2.2.0-Windows-x64-Setup.exe)

Windows 10/11, x64
Запустите EXE, выберите папку и нужные ярлыки
Автозапуск можно включить при установке или позже в настройках приложения
Установщик сохраняет подписки и пользовательские настройки

## macOS

[![Скачать DMG 1.0.0 для macOS](assets/download-macos-dmg.svg)](https://github.com/WireonWN/H-Connect/releases/download/macos-v1.0.0/HorizonConnect-1.0.0-macOS-arm64.dmg)

Требуется macOS 15 или новее и Mac с Apple Silicon

1. Откройте DMG и перетащите Horizon Connect в «Программы»
2. Запустите приложение из «Программ» и добавьте подписку или конфиг
3. При первом подключении разрешите системное расширение, если macOS покажет запрос

[Что вошло в первый выпуск](docs/MACOS.md)

## Linux

Версия **2.2.0**, архитектура **x86_64**, ядро **AirX**, Qt включён в комплект

Минимум: glibc 2.35, Python 3 и OpenSSL 3
Manjaro использует пакет Arch при совместимых системных зависимостях
Сборка не предназначена для ARM, 32-битных систем и дистрибутивов на musl, например Alpine

### Debian / Ubuntu

```sh
sudo apt install ./HorizonConnect-2.2.0-Linux-amd64.deb
```

### Fedora

```sh
sudo dnf install ./HorizonConnect-2.2.0-Linux-x86_64.rpm
```

### Arch / Manjaro

```sh
sudo pacman -U ./HorizonConnect-2.2.0-Linux-x86_64.pkg.tar.zst
```

Команды выполняются из папки со скачанным пакетом
Менеджер пакетов установит зависимости
Запускайте приложение из меню рабочего стола или командой `horizon-connect` от обычного пользователя

### ZIP

ZIP содержит переносимый комплект приложения, включая Qt

```sh
unzip HorizonConnect-2.2.0-Linux-x86_64.zip
cd HorizonConnect-2.2.0-Linux-x86_64
./horizon-connect
```

Для ZIP системные зависимости устанавливаются отдельно: Python 3, glibc ≥ 2.35, libstdc++ ≥ 11, OpenSSL 3, Kerberos, OpenGL/EGL, GLib, D-Bus, Fontconfig/FreeType, X11/XCB, xkbcommon, Wayland, zlib/zstd и polkit для системного TUN
Для поддерживаемых пакетных систем проще использовать соответствующий пакет: он содержит точный список зависимостей

При первом запуске любой Linux-сборки рабочий комплект создаётся в `~/.local/opt/horizon-connect/bin`
Этот каталог используется обновлением из приложения; запускать GUI через `sudo` не нужно

[Как работают обновления и где хранятся данные](docs/UPDATES.md)

## Зеркало и контрольные суммы

[Файлы на сервере и SHA256SUMS](docs/RELEASE-2026-11-18.md#прямые-загрузки)
Сверяйте скачанный файл с контрольной суммой соответствующего релиза

## Первое подключение

1. Добавьте подписку или конфигурацию сервера
2. Выберите сервер
3. Запустите подключение
4. Подтвердите системный запрос VPN, если он появится

## Файлы релиза

| Обозначение | Назначение |
| :--- | :--- |
| Assets | Файлы приложения, прикреплённые к релизу |
| Source code | Архив содержимого репозитория, не установщик |
| Pre-release | Тестовая версия |

## Ошибка установки

[Создайте обращение](https://github.com/WireonWN/H-Connect/issues/new/choose)
Укажите систему, архитектуру, версию приложения и текст ошибки
