# Task A — детекция ключевого слова в аудио

**Результат:** leaderboard score `0.975`, validation accuracy `97.64%`.

## Решение

- предобученный `wav2vec2-large-xlsr-53-russian`;
- единый семплинг 16 kHz и ограничение записи до 5 секунд;
- fine-tuning всей модели с небольшим learning rate;
- стратифицированное разделение на train/validation;
- сохранение лучшего чекпоинта по validation accuracy.

## Данные

```text
data/
├── train/
│   ├── word_bounds.json
│   └── audio/*.opus
└── test/
    └── audio/*.opus
```

Запустите `solution.ipynb`. Итоговый файл: `outputs/final_submission.csv`.
