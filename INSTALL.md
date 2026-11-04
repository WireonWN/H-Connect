[Horizon Connect](README.md) / Установка

# Загрузка и установка

## Загрузка

| Система | Сборки | Инструкция |
| :--- | :--- | :--- |
| Android | [![APK](assets/badge-apk.svg)](https://github.com/WireonWN/H-Connect/releases) [![Google Play](assets/badge-play.svg)](https://play.google.com/store/apps/details?id=com.horizon.connect) | [Android](#android) |
| Windows | [![Windows .exe](assets/download-windows-exe.svg)](https://github.com/WireonWN/H-Connect/releases/download/windows-v2.0.0/HorizonConnect-2.0.0-Setup.exe) | [Windows](#windows) |
| Linux | [![Debian / Ubuntu .deb](assets/download-linux-deb.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v1.0.0/HorizonConnect-1.0.0-linux-amd64.deb) <br /> [![Fedora .rpm](assets/download-linux-rpm.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v1.0.0/HorizonConnect-1.0.0-linux-x86_64.rpm) <br /> [![Arch / Manjaro .pkg.tar.zst](assets/download-linux-arch.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v1.0.0/HorizonConnect-1.0.0-linux-arch-x86_64.pkg.tar.zst) <br /> [![Linux .zip](assets/download-linux-zip.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v1.0.0/HorizonConnect-v1.0-Linux-Installers.zip) | [Linux](#linux) |

Файлы конкретной версии находятся в **Assets** её релиза

## Android

**Google Play**

1. Откройте [страницу Horizon Connect](https://play.google.com/store/apps/details?id=com.horizon.connect)
2. Установите приложение или выберите обновление

**APK**

Android APK будет добавлен отдельным релизом
После публикации:

1. Скачайте APK из **Assets**
2. Откройте файл на устройстве
3. Разрешите установку из выбранного источника, если система запросит доступ
4. Завершите установку

Для обновления используйте тот же источник установки

## Windows

[Скачать Horizon Connect 2.0.0 для Windows](https://github.com/WireonWN/H-Connect/releases/download/windows-v2.0.0/HorizonConnect-2.0.0-Setup.exe)

1. Скачайте EXE-установщик
2. Запустите его и выполните шаги установки
3. Откройте Horizon Connect и добавьте конфигурацию подключения

[Описание выпуска и контрольная сумма](https://github.com/WireonWN/H-Connect/releases/tag/windows-v2.0.0)

## Linux

Версия **1.0.0**, архитектура **x86_64**, ядро **Mihomo**
ZIP содержит все три пакета и инструкцию, для установки достаточно скачать один пакет своей системы

### Debian / Ubuntu

```sh
sudo apt install ./HorizonConnect-1.0.0-linux-amd64.deb
```

### Fedora / RPM

```sh
sudo dnf install ./HorizonConnect-1.0.0-linux-x86_64.rpm
```

### Arch / Manjaro

```sh
sudo pacman -U ./HorizonConnect-1.0.0-linux-arch-x86_64.pkg.tar.zst
```

Команды выполняются из папки со скачанным пакетом
DEB-пакет указывает зависимость glibc 2.35 или новее, остальные зависимости устанавливаются менеджером пакетов

[Описание выпуска и контрольные суммы](https://github.com/WireonWN/H-Connect/releases/tag/linux-v1.0.0)

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
