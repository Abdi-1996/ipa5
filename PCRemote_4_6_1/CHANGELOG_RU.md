# PC Remote 4.6.1.1

## CorelDRAW Remote

- CorelDRAW распознается как специальная интеграция.
- Нажатие на CorelDRAW запускает приложение на ПК и одновременно открывает нативный модуль на iPhone.
- Новый iOS/glass интерфейс CorelDRAW с живым предпросмотром документа.
- Список объектов, выбор объекта и контекстные настройки.
- Положение, размер, сохранение пропорций и поворот.
- Заливка и контур с быстрыми цветами.
- Создание rectangle / ellipse / artistic text / line.
- Duplicate, Delete, Group, Ungroup, Bring to Front, Send to Back.
- Undo / Redo и выбор всех объектов.
- Управление страницами.
- Открытие файлов CorelDRAW и совместимых векторных форматов через Проводник PC Remote.
- Отдельная кнопка для показа полного CorelDRAW на Windows.

## Сборка

- `.github/workflows/main.yml` теперь универсальный и не привязан к номеру версии/имени папки.
- Артефакты всегда называются `PCRemote-IPA` и `PCRemote-Windows`.
- ATS-проверка LAN/Tailscale выполняется непосредственно на собранном `.app` перед упаковкой IPA.
- Windows EXE включает `corel_bridge.py` и `comtypes` для автоматизации CorelDRAW.
