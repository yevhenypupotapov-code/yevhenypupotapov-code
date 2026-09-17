# ContentForge 🛠️ — контент-фабрика на твоём ПК

<p align="center">
  <img src="assets/banner.svg" alt="ContentForge — локальная контент-фабрика: Ollama, ComfyUI + LTXV, FFmpeg, Windows SAPI, YouTube API" width="100%">
</p>

<p align="center">
  <a href="https://github.com/yevhenypupotapov-code/contentforge/releases"><img src="https://img.shields.io/github/v/release/yevhenypupotapov-code/contentforge?style=flat-square&label=%D1%80%D0%B5%D0%BB%D0%B8%D0%B7" alt="Release"></a>
  <a href="https://github.com/yevhenypupotapov-code/contentforge/blob/main/LICENSE"><img src="src="https://img.shields.io/badge/license-Proprietary-b3402a?style=flat-square" alt="License: Proprietary">></a>
  <img src="https://img.shields.io/badge/platform-Windows-0078D4?style=flat-square" alt="Platform: Windows">
  <img src="https://img.shields.io/badge/%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8-%D0%BB%D0%BE%D0%BA%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5-b3402a?style=flat-square" alt="Local models only">
  <a href="https://www.youtube.com/@yevhenpotapov5956"><img src="https://img.shields.io/badge/YouTube-%40yevhenpotapov5956-FF0000?style=flat-square&logo=youtube&logoColor=white" alt="YouTube"></a>
</p>

Две автономные контент-фабрики, которые работают на обычном ПК и сами выпускают видео:
берут актуальные тренды, пишут сценарий, генерируют кадры и анимацию, озвучивают, монтируют
и публикуют выпуск на YouTube. **Всё создаётся локально** — из интернета приходят только
тренды и загрузка готового ролика.

**Твоё, без облака.** Никаких внешних генераторов текста, картинок или голоса: сценарий считает
локальная модель, кадры рисует ComfyUI, голос даёт системный синтез речи Windows.

---

## Что внутри

| Завод | Что делает | Формат | Расписание |
|---|---|---|---|
| **Long** | Длинный выпуск: тема → сценарий → кадры и LTXV-клипы → сборка → публикация | 16:9, ~1 минута | Пт, Сб — 11:00 и 18:00 |
| **Shorts** | Короткий ролик с текстом на кадре | 9:16, до 30 секунд | Пт, Сб — 07:00, 15:00, 23:00 |

Оба публикуют выпуски **в открытом доступе** и только по пятницам и субботам.

## Как это работает

```text
тренды → сценарий → раскадровка → кадры и видео → озвучка → монтаж → публикация → уведомление
 (сеть)    (Ollama)     (Ollama)     (ComfyUI+LTXV)  (SAPI)    (FFmpeg)   (YouTube)    (Telegram)
```

Каждый выпуск получает свой визуальный облик: цветовой грейд из ротации, в которой последние
шесть выпусков не повторяются. Плюс защита от дублей, проверка «чёрных кадров», удержание
кадра и разнообразие сцен.

## Быстрый старт

1. Скачать архив приложения из [релиза](https://github.com/yevhenypupotapov-code/contentforge/releases).
2. Распаковать в любую папку.
3. Запустить `ContentForge.bat`.
4. Пункт **«Проверить этот ПК»** — покажет, всё ли на месте.

Нужны: Windows 10/11, Python 3.10+, FFmpeg, [Ollama](https://ollama.com), ComfyUI с LTXV
и NVIDIA GPU от 8 ГБ.

## Проекты

- **[contentforge](https://github.com/yevhenypupotapov-code/contentforge)** — приложение и веб-панель управления заводом
- **[ltx-youtube-gold-standard](https://github.com/yevhenypupotapov-code/ltx-youtube-gold-standard)** — ядро длинного завода: сборка, гейты качества, генерация кадров

## Канал

Выпуски выходят на **[YEVHEN POTAPOV](https://www.youtube.com/@yevhenpotapov5956)**.

<p align="center"><sub>© 2026 Yevhen Potapov · Все права защищены · Локальные модели · Windows</sub></p>
