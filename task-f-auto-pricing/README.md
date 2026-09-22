# Task F — оценка стоимости автомобиля

**Результат:** leaderboard score `0.820`; validation median APE `0.2082`.

## Решение

- очистка и нормализация табличных признаков автомобиля;
- визуальные эмбеддинги до четырёх фотографий на объект;
- агрегация эмбеддингов усреднением;
- CatBoostRegressor в логарифмическом пространстве цены;
- подбор мультипликативной поправки на validation.

## Данные

```text
data/
├── train_dataset.parquet
├── test_dataset.parquet
├── sample_submission.csv
├── train_images/
└── test_images/
```

Запустите `solution.ipynb`; эмбеддинги и `submission.csv` будут сохранены в `outputs/`.
