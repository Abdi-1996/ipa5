# PC Remote 4.4.1 — ATS HTTP Fix

Исправление для iOS App Transport Security.

## Что изменено

- В `Info.plist` добавлен `NSAllowsArbitraryLoads = YES` вместе с `NSAllowsLocalNetworking = YES`.
- Это разрешает PC Remote обращаться к вашему PC Remote Server по HTTP напрямую на LAN IP (`192.168.x.x`) и Tailscale IP (`100.x.x.x`).
- Версия приложения: `4.4.1`, build `7`.
- GitHub Actions создаёт `PCRemote-4.4.1-IPA` и `PCRemote-4.4.1-Windows`.

## Проверка после установки

1. Запустите PC Remote Server на Windows.
2. Сначала проверьте вход по LAN.
3. Затем включите Tailscale на iPhone и выберите режим Tailscale/Auto.
4. Для проверки удалённого доступа отключите Wi‑Fi на iPhone и попробуйте подключиться через мобильную сеть.
