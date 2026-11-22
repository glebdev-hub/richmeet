# How to install RichMeet

Requires a Mac with Apple silicon (M1 or later) and macOS 26 or later. About 5 GB of free space (app + models).

## Install
1. Open `RichMeet-<version>.dmg`.
2. Drag **RichMeet** into the **Applications** folder.
3. Eject the RichMeet disk.

## First launch
The app isn't notarized by Apple yet, so macOS will block it the first time. You only need to do this once.

1. Open RichMeet from Applications. A message says it can't be verified — click **Done**.
2. Open **System Settings → Privacy & Security**.
3. Scroll down to **Security** and click **Open Anyway** next to RichMeet, then confirm with your password.
4. Open RichMeet again and click **Open**.

For advanced users, the same in Terminal:
`xattr -dr com.apple.quarantine /Applications/RichMeet.app`

## Next steps
- Accept the User Agreement. The app then offers to download a model for translation and summaries (about 3 GB) and asks for permissions:
  **Microphone** — for your speech; **Screen & System Audio Recording** — for other people's speech. You may need to restart the app after granting the second one.
- The RichMeet icon appears in the menu bar at the top of the screen.
- The interface follows your macOS language (English, French, German, Italian, Spanish, Russian or Thai).

## Updating
Download the new .dmg and replace the app in Applications. Recordings and models are kept.
Until the app is signed with an Apple certificate, macOS may ask for microphone and audio permission again after an update.

## Uninstalling
Settings → “Recordings & Shortcuts” → “Delete all data”, then drag the app from Applications to the Trash.

---

# Как установить RichMeet

Требуется Mac с Apple Silicon (M1 и новее) и macOS 26 или новее. Нужно около 5 ГБ свободного места (приложение + модели).

## Установка
1. Откройте файл `RichMeet-<версия>.dmg`.
2. Перетащите **RichMeet** в папку **Программы** (Applications).
3. Извлеките диск RichMeet.

## Первый запуск
Приложение пока не заверено Apple (нет нотаризации), поэтому macOS при первом запуске его остановит. Это делается один раз.

1. Откройте RichMeet из «Программ». Появится сообщение, что приложение не удаётся проверить — нажмите **Готово**.
2. Откройте **Системные настройки → Конфиденциальность и безопасность**.
3. Внизу, в разделе «Безопасность», нажмите **Всё равно открыть** рядом с RichMeet и подтвердите паролем.
4. Запустите RichMeet ещё раз и нажмите **Открыть**.

Для опытных: то же самое одной командой в Терминале —
`xattr -dr com.apple.quarantine /Applications/RichMeet.app`

## Дальше
- Приложение предложит скачать модель для перевода и конспектов (около 3 ГБ) и попросит разрешения:
  **Микрофон** — для вашей речи; **Запись экрана и системного звука** — для речи собеседников. После выдачи второго разрешения может понадобиться перезапустить приложение.
- Значок RichMeet появится в строке меню вверху экрана.

## Обновление
Скачайте новый .dmg и замените приложение в «Программах». Записи и модели сохранятся.
Пока приложение не подписано сертификатом Apple, после обновления macOS может заново спросить разрешения на микрофон и звук.

## Удаление
Настройки → «Записи и клавиши» → «Удалить все данные», затем перетащите приложение из «Программ» в Корзину.
