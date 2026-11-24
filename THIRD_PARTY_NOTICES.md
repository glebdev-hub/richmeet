# Сторонние компоненты RichMeet

## Входят в приложение

| Компонент | Автор | Лицензия | Где |
|---|---|---|---|
| llama.cpp (llama-server, ggml; в сборке для App Store — статическая библиотека внутри приложения, тег b12559) | ggml-org и участники | MIT | https://github.com/ggml-org/llama.cpp |
| ZIPFoundation 0.9.20 (чтение .xlsx/.pptx в базе знаний) | Thomas Zoechling | MIT | https://github.com/weichsel/ZIPFoundation |
| WhisperKit, SpeakerKit | Argmax, Inc. | MIT | https://github.com/argmaxinc/WhisperKit (своя копия 1.1.1 с изменённой кластеризацией голосов — `Packages/WhisperKit`) |
| Swift Argument Parser | Apple Inc. | Apache 2.0 | https://github.com/apple/swift-argument-parser |

Тексты лицензий лежат рядом с этим файлом.

## Скачиваются по запросу пользователя

| Модель | Автор | Лицензия | Где |
|---|---|---|---|
| Gemma 4 E2B / E4B (GGUF) | Google; квантование Unsloth, LM Studio, bartowski | Apache 2.0 | https://ai.google.dev/gemma/docs/gemma_4_license |
| Whisper large-v3-turbo (Core ML) | OpenAI; конвертация Argmax | MIT | https://huggingface.co/argmaxinc/whisperkit-coreml |
| multilingual-e5-small (GGUF), поиск по смыслу в базе знаний | Microsoft (intfloat); конвертация TwinSunsLLC | MIT | https://huggingface.co/intfloat/multilingual-e5-small |
| Разделение голосов (Core ML) | pyannote (сегментация, кластеризация), WeSpeaker (эмбеддинги); конвертация Argmax | MIT / CC BY 4.0 | https://huggingface.co/argmaxinc/speakerkit-coreml |

Модели не входят в установщик. В сборке для App Store они скачиваются из пакетов Apple-hosted Background Assets (те же файлы и лицензии), а если пакетов нет — с Hugging Face с проверкой SHA-256. Разделение голосов в сборке для App Store выключено и включается только экспериментальным флагом: эмбеддер WeSpeaker обучен на VoxCeleb, который выдан «для исследований».

## Системные компоненты macOS
Распознавание речи (Speech / SpeechAnalyzer), перевод (Translation), запись звука (ScreenCaptureKit, AVFoundation) — фреймворки Apple, входят в macOS.
