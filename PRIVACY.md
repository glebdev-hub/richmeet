# Конфиденциальность RichMeet

Актуальная версия: https://glebdev-hub.github.io/richmeet/PRIVACY · Версия от 24 ноября 2026 г. (для RichMeet из Mac App Store)

Коротко: всё, что вы говорите и слушаете, остаётся на вашем Mac. Разработчик не собирает никаких данных.

**Что обрабатывается и где**
- Звук микрофона и компьютера распознаётся системными средствами macOS (SpeechAnalyzer) на устройстве.
- Перевод выполняет системный переводчик Apple (на устройстве) или встроенная языковая модель (llama.cpp внутри приложения), которая работает на этом Mac.
- Точная расшифровка (Whisper), конспекты, отчёты, ответы на вопросы и поиск по базе знаний делаются локально.
- RichMeet работает в песочнице App Store (App Sandbox): он видит только свою папку данных и те папки и файлы, которые вы сами выбрали.

**Что хранится и где**
- Записи встреч, расшифровки, конспекты и заметки — в папке данных RichMeet (контейнер приложения) или в папке, которую вы выбрали в настройках.
- Модели, индекс базы знаний и настройки — в контейнере приложения и в общей папке группы приложений RichMeet (~/Library/Group Containers) — её же читает MCP-сервер RichMeet.
- Документы базы знаний остаются в своих папках; RichMeet только читает их (с вашего разрешения) и хранит текстовый индекс. Сканы распознаются системными средствами macOS (Vision) на устройстве.
- Если вы включите экспериментальное разделение голосов и «Запоминать голоса», отпечатки голосов собеседников, которым вы дали имя, хранятся в папке данных RichMeet. Это биометрические данные: они не покидают Mac; удалить — Настройки → «Встречи» → «Забыть все голоса».

Всё это можно удалить в Настройках → «Записи и клавиши» → «Удалить все данные» или удалив приложение.

**Что уходит в интернет**
- Скачивание моделей: из пакетов Apple (Background Assets, серверы Apple), а если они недоступны — с Hugging Face (huggingface.co) с проверкой целостности. Передаётся только запрос файла модели.
- Языковые пакеты распознавания и перевода macOS скачивает с серверов Apple по правилам Apple.
- Покупки и подписки проходят через App Store (StoreKit). Оплату обрабатывает Apple; у RichMeet нет своих серверов, и разработчик не получает ваших платёжных или личных данных — только обезличенные отчёты о продажах от Apple.
- Никакой аналитики, рекламы, отчётов о сбоях от разработчика и учётных записей.
- **ИИ-помощники через MCP — только если вы их подключите.** MCP-сервер RichMeet работает на вашем Mac и только читает данные. Если добавить RichMeet в Claude Desktop, Claude Code или другой помощник (Настройки → «Модель» → «Доступ для ИИ-помощников»), помощник сможет читать конспекты, задачи, заметки и расшифровки (без звука) и отправлять прочитанное своему провайдеру по его правилам. RichMeet сам ничего не отправляет.
- **Облачные модели — только если вы их включите.** Если в Настройках → «Модель» выбрать Claude, OpenAI, DeepSeek или Kimi и ввести свой API-ключ, текст расшифровок, заметок, вопросов и найденных фрагментов документов базы знаний отправляется этому провайдеру и обрабатывается по его правилам (серверы DeepSeek и Kimi — в Китае). Звук и в этом случае остаётся на Mac. Ключ хранится в связке ключей macOS.

**Запись собеседников**
Перед записью созвона предупредите участников: в ряде стран запись разговора без согласия запрещена.

**Связь**
Вопросы о конфиденциальности: https://github.com/glebdev-hub/richmeet/issues

---

# RichMeet Privacy Policy

Latest version: https://glebdev-hub.github.io/richmeet/PRIVACY · Version of November 24, 2026 (for RichMeet from the Mac App Store)

In short: everything you say and hear stays on your Mac. The developer collects no data.

**What is processed and where**
- Microphone and computer audio is recognized on device by macOS (SpeechAnalyzer).
- Translation is done by Apple Translate (on device) or by the built-in language model (llama.cpp inside the app) running on this Mac.
- Accurate transcription (Whisper), summaries, reports, answers to questions and knowledge-base search are all local.
- RichMeet runs in the App Store sandbox (App Sandbox): it can access only its own data folder and the folders and files you choose.

**What is stored and where**
- Meeting recordings, transcripts, summaries and notes — in RichMeet's data folder (the app container) or in a folder you chose in Settings.
- Models, the knowledge-base index and settings — in the app container and in the shared RichMeet app-group folder (~/Library/Group Containers), which the RichMeet MCP server also reads.
- Knowledge-base documents stay in their folders; RichMeet only reads them (with your permission) and keeps a text index. Scans are recognized on device by macOS (Vision).
- If you turn on experimental speaker separation and “Remember speakers' voices”, voiceprints of speakers you named are stored in RichMeet's data folder. This is biometric data: it never leaves your Mac; delete it in Settings → “Meetings” → “Forget all voices”.

You can delete all of it in Settings → “Recordings & Shortcuts” → “Delete all data”, or by deleting the app.

**What goes to the internet**
- Model downloads: from Apple-hosted asset packs (Background Assets, Apple servers), or, if unavailable, from Hugging Face (huggingface.co) with an integrity check. Only the request for the model file is sent.
- macOS downloads speech-recognition and translation language packs from Apple under Apple's terms.
- Purchases and subscriptions go through the App Store (StoreKit). Apple processes payments; RichMeet has no servers of its own, and the developer receives none of your payment or personal data — only anonymized sales reports from Apple.
- No analytics, ads, developer crash reports or accounts.
- **AI assistants via MCP — only if you connect them.** The RichMeet MCP server runs on your Mac and is read-only. If you add RichMeet to Claude Desktop, Claude Code or another assistant (Settings → “Model” → “Access for AI assistants”), the assistant can read summaries, tasks, notes and transcripts (no audio) and send what it reads to its provider under its terms. RichMeet itself sends nothing.
- **Cloud models — only if you turn them on.** If you choose Claude, OpenAI, DeepSeek or Kimi in Settings → “Model” and enter your own API key, the text of transcripts, notes, questions and matching fragments of knowledge-base documents is sent to that provider and handled under its terms (DeepSeek and Kimi servers are in China). Audio still stays on your Mac. The key is stored in the macOS Keychain.

**Recording other people**
Tell participants before recording a call: in some countries recording a conversation without consent is illegal.

**Contact**
Privacy questions: https://github.com/glebdev-hub/richmeet/issues
