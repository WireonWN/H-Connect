<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/wordmark-dark.png" />
    <source media="(prefers-color-scheme: light)" srcset="assets/wordmark-light.png" />
    <img src="assets/wordmark-light.png" alt="Horizon Connect" width="640" />
  </picture>
</p>

<p align="center">
  <a href="#ядро-airx"><img src="assets/badge-airx.svg" alt="Core: AirX" /></a>
  <a href="INSTALL.md"><img src="assets/badge-platforms.svg" alt="Android, Windows, Linux" /></a>
  <a href="https://play.google.com/store/apps/details?id=com.horizon.connect"><img src="assets/badge-play.svg" alt="Google Play: Android" /></a>
  <br />
  <a href="https://play.google.com/store/apps/details?id=com.horizon.connect"><img src="assets/stats-installs-30000.svg" alt="Google Play: 30 000 скачиваний" /></a>
  <a href="https://play.google.com/store/apps/details?id=com.horizon.connect"><img src="assets/stats-active-25000.svg" alt="25 000 активных пользователей за месяц" /></a>
</p>

<p align="center">
  <a href="INSTALL.md"><strong>Установка</strong></a> ·
  <a href="https://github.com/WireonWN/H-Connect/releases"><strong>Релизы</strong></a> ·
  <a href="https://github.com/WireonWN/H-Connect/issues"><strong>Обратная связь</strong></a>
</p>

## Horizon Connect

Клиент для подключения по собственной конфигурации или подписке
Добавьте ссылку, выберите сервер и запустите соединение

## Загрузка

| Платформа | Загрузка | Установка |
| :--- | :--- | :--- |
| **Android** | [![APK](assets/badge-apk.svg)](https://github.com/WireonWN/H-Connect/releases/download/android-v2.3.0/HorizonConnect-2.3.0-Android.apk) [![Google Play](assets/badge-play.svg)](https://play.google.com/store/apps/details?id=com.horizon.connect) | [Инструкция](INSTALL.md#android) |
| **Windows** | [![Windows .exe](assets/download-windows-exe.svg)](https://github.com/WireonWN/H-Connect/releases/download/windows-v2.1.1/HorizonConnect-2.1.1-Windows-x64-Setup.exe) | [Инструкция](INSTALL.md#windows) |
| **Linux** | [![Debian / Ubuntu .deb](assets/download-linux-deb.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v2.1.1/HorizonConnect-2.1.1-Linux-amd64.deb) <br /> [![Fedora .rpm](assets/download-linux-rpm.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v2.1.1/HorizonConnect-2.1.1-Linux-x86_64.rpm) <br /> [![Arch / Manjaro .pkg.tar.zst](assets/download-linux-arch.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v2.1.1/HorizonConnect-2.1.1-Linux-x86_64.pkg.tar.zst) <br /> [![Linux .zip](assets/download-linux-zip.svg)](https://github.com/WireonWN/H-Connect/releases/download/linux-v2.1.1/HorizonConnect-2.1.1-Linux-x86_64.zip) | [Инструкция](INSTALL.md#linux) |

## Версии

| Платформа | Выпуск | Ветка |
| :--- | :--- | :--- |
| Windows | [2.1.1](https://github.com/WireonWN/H-Connect/releases/tag/windows-v2.1.1) | [![Ветка windows](assets/branch-windows.svg)](https://github.com/WireonWN/H-Connect/tree/windows) |
| Linux | [2.1.1](https://github.com/WireonWN/H-Connect/releases/tag/linux-v2.1.1) | [![Ветка linux](assets/branch-linux.svg)](https://github.com/WireonWN/H-Connect/tree/linux) |
| Android | [2.3.0](https://github.com/WireonWN/H-Connect/releases/tag/android-v2.3.0) | [![APK](assets/badge-apk.svg)](https://github.com/WireonWN/H-Connect/releases/download/android-v2.3.0/HorizonConnect-2.3.0-Android.apk) [![Google Play](assets/badge-play.svg)](https://play.google.com/store/apps/details?id=com.horizon.connect) |

[Что изменилось в выпуске](docs/RELEASE-2026-11-13.md) · [Обновления приложения](docs/UPDATES.md)

## Возможности

- **Раздельное туннелирование**: выбор приложений, которые работают в обход VPN
- **Маршрутизация по доменам**: исключения для отдельных сайтов и доменных зон
- **Пользовательский DNS**: выбор DNS-сервера и настройка разрешения имён
- **Локальный SOCKS5**: подключение других устройств к активному VPN через локальную сеть, с настройкой порта и авторизации
- **Автоподключение**: автоматический запуск соединения с выбранным режимом выбора сервера
- **Управление по блокировке экрана**: отключение VPN при блокировке и восстановление после разблокировки
- **Настройка MTU**: выбор размера пакетов туннеля
- **IPv6**: управление передачей IPv6-трафика внутри туннеля
- **Параметры TLS и транспорта**: настройка соединения для выбранного протокола

## Протоколы

| Протокол | Режимы и особенности |
| :--- | :--- |
| VLESS | REALITY, TLS, TCP, gRPC, XHTTP |
| VMess | AEAD |
| Trojan | TLS |
| Shadowsocks 2022 | AES-128-GCM, AES-256-GCM |
| Hysteria2 | TCP и UDP, обфускация Salamander |
| TUIC v5 | TCP, UDP native и UDP через QUIC stream |
| NaiveProxy | HTTPS-прокси |
| WireGuard | UDP-туннель |
| AmneziaWG | Версии 1, 1.5, 2, 3 и 3.1 |
| OpenVPN | TCP и UDP |
| IKEv2/IPsec | PSK, сертификаты, EAP-MSCHAPv2 |
| SSH Tunnel | Туннелирование через SSH |

## Ядро AirX

**AirX** отвечает за сетевую часть Horizon Connect
Основная логика ядра написана на Rust

- Подключение к серверам и работа протоколов
- Передача TCP- и UDP-трафика
- Обработка DNS и правил маршрутизации
- Управление состоянием соединения

Версии приложения и ядра обновляются отдельно

[Подробнее о возможностях AirX](docs/AIRX.md)

## Обратная связь

[Сообщить об ошибке](https://github.com/WireonWN/H-Connect/issues/new/choose) / [Предложить улучшение](https://github.com/WireonWN/H-Connect/issues/new)

Для разбора ошибки укажите систему, версию приложения, протокол и шаги воспроизведения
При необходимости приложите скриншот или фрагмент журнала без паролей, ключей и ссылок подписок
