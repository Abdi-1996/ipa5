# PC Remote 4.5.1 — ATS Force Fix

Исправление предназначено для ошибки iOS:

`The resource could not be loaded because the App Transport Security policy requires the use of a secure connection.`

Что изменено:
- `Info.plist` target PCRemote содержит `NSAllowsArbitraryLoads = true` и `NSAllowsLocalNetworking = true`.
- Xcode target явно использует `PCRemote/Info.plist` (`GENERATE_INFOPLIST_FILE = NO`).
- GitHub Actions после компиляции принудительно проверяет и, при необходимости, записывает ATS-ключи прямо в итоговый `PCRemote.app/Info.plist`.
- Сборка останавливается, если итоговый `.app` не содержит `NSAllowsArbitraryLoads = true`.
- Версия: 4.5.1, build 9.

После установки можно использовать HTTP-сервер PC Remote по LAN `192.168.x.x:8765` и через Tailscale `100.x.x.x:8765`.
