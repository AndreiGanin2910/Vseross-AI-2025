# Task D — прогноз габаритов товара

**Результат:** leaderboard score `0.764`.

## Решение

- TF-IDF по текстовым и категориальным полям + Truncated SVD;
- SigLIP-эмбеддинги изображений + Truncated SVD;
- статистики размеров внутри микрокатегорий;
- отдельный CatBoostRegressor для веса, высоты, длины и ширины;
- log1p-преобразование целевых значений.

## Данные

```text
data/
├── train.parquet
├── test.parquet
├── sample_submission.csv
├── train_images/
└── test_images/
```

Запустите `solution.ipynb`; результат будет сохранён в `outputs/submission_siglip_hybrid.csv`.
