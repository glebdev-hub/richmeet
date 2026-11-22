# Сторонние компоненты RichMeet

## Входят в приложение

| Компонент | Автор | Лицензия | Где |
|---|---|---|---|
| llama.cpp (llama-server, ggml) | ggml-org и участники | MIT | https://github.com/ggml-org/llama.cpp |
| WhisperKit, SpeakerKit | Argmax, Inc. | MIT | https://github.com/argmaxinc/WhisperKit (своя копия 1.1.1 с изменённой кластеризацией голосов — `Packages/WhisperKit`) |
| Swift Argument Parser | Apple Inc. | Apache 2.0 | https://github.com/apple/swift-argument-parser |

Тексты лицензий лежат рядом с этим файлом.

## Скачиваются по запросу пользователя

| Модель | Автор | Лицензия | Где |
|---|---|---|---|
| Gemma 4 E2B / E4B (GGUF) | Google; квантование Unsloth, LM Studio, bartowski | Apache 2.0 | https://ai.google.dev/gemma/docs/gemma_4_license |
| Whisper large-v3-turbo (Core ML) | OpenAI; конвертация Argmax | MIT | https://huggingface.co/argmaxinc/whisperkit-coreml |
| Разделение голосов (Core ML) | pyannote (сегментация, кластеризация), WeSpeaker (эмбеддинги); конвертация Argmax | MIT / CC BY 4.0 | https://huggingface.co/argmaxinc/speakerkit-coreml |

Модели не входят в установщик и скачиваются с Hugging Face при первом использовании.

## Системные компоненты macOS
Распознавание речи (Speech / SpeechAnalyzer), перевод (Translation), запись звука (ScreenCaptureKit, AVFoundation) — фреймворки Apple, входят в macOS.
