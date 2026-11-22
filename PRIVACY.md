# Конфиденциальность RichMeet

Актуальная версия: https://glebdev-hub.github.io/richmeet/PRIVACY

Коротко: всё, что вы говорите и слушаете, остаётся на вашем Mac.

**Что обрабатывается и где**
- Звук микрофона и компьютера распознаётся системными средствами macOS (SpeechAnalyzer) на устройстве.
- Перевод выполняется либо системным переводчиком Apple (на устройстве), либо встроенной моделью (llama.cpp), которая работает на этом Mac.
- Точная расшифровка (Whisper), разделение голосов, конспекты и ответы на вопросы делаются локально.

**Что хранится**
- Записи встреч, расшифровки, конспекты и заметки — в папке, выбранной в настройках (по умолчанию «Документы/iRichAudio Transcripts»).
- Модели — в «~/Library/Application Support/iRichAudio».
- Настройки — в стандартных настройках macOS.

- Отпечатки голосов собеседников, которым вы дали имя (если включено «Запоминать голоса»), — в «~/Library/Application Support/iRichAudio/voices.json» и рядом с записями встреч. Это биометрические данные: они не покидают Mac; удалить — Настройки → «Встречи» → «Забыть все голоса».

Всё это можно удалить в Настройках → «Записи и клавиши» → «Удалить все данные».

**Что уходит в интернет**
- Только скачивание моделей с Hugging Face (huggingface.co) — когда вы сами их скачиваете или при первой расшифровке Whisper.
- Никакой аналитики, отчётов о сбоях, рекламы и учётных записей.
- **Облачные модели — только если вы их включите.** Если в Настройках → «Модель» выбрать Claude, OpenAI, DeepSeek или Kimi и ввести свой API-ключ, текст расшифровок, заметок и вопросов отправляется этому провайдеру и обрабатывается по его правилам (серверы DeepSeek и Kimi — в Китае). Звук и в этом случае остаётся на Mac. Ключ хранится в связке ключей macOS.

**Запись собеседников**
Перед записью созвона предупредите участников: в ряде стран запись разговора без согласия запрещена.

---

# RichMeet Privacy

Latest version: https://glebdev-hub.github.io/richmeet/PRIVACY

In short: everything you say and hear stays on your Mac.

**What is processed and where**
- Microphone and computer audio is recognized on device by macOS (SpeechAnalyzer).
- Translation is done either by Apple Translate (on device) or by the built-in model (llama.cpp) running on this Mac.
- Accurate transcription (Whisper), speaker separation, summaries and answers to questions are all local.

**What is stored**
- Meeting recordings, transcripts, summaries and notes — in the folder chosen in Settings (by default “Documents/iRichAudio Transcripts”).
- Models — in “~/Library/Application Support/iRichAudio”.
- Settings — in standard macOS preferences.

- Voiceprints of speakers you named (if “Remember speakers' voices” is on) — in “~/Library/Application Support/iRichAudio/voices.json” and next to meeting recordings. This is biometric data: it never leaves your Mac; delete it in Settings → “Meetings” → “Forget all voices”.

You can delete all of it in Settings → “Recordings & Shortcuts” → “Delete all data”.

**What goes to the internet**
- Only model downloads from Hugging Face (huggingface.co) — when you download them yourself or on the first Whisper transcription.
- No analytics, crash reports, ads or accounts.
- **Cloud models — only if you turn them on.** If you choose Claude, OpenAI, DeepSeek or Kimi in Settings → “Model” and enter your own API key, the text of transcripts, notes and questions is sent to that provider and handled under its terms (DeepSeek and Kimi servers are in China). Audio still stays on your Mac. The key is stored in the macOS Keychain.

**Recording other people**
Tell participants before recording a call: in some countries recording a conversation without consent is illegal.
