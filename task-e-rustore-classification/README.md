# Task E — классификация приложений RuStore

**Результат:** Hitrate@3 `0.926`.

## Решение

- структурирование названия, короткого и полного описания приложения;
- fine-tuning `DeepPavlov/rubert-base-cased`;
- multilabel BCEWithLogitsLoss;
- cosine scheduler, gradient clipping и выбор лучшего чекпоинта;
- top-3 классов по вероятности для каждого приложения.

Положите `train.tsv` и `test.tsv` в `data/`. Запустите `solution.ipynb`; итоговый файл — `outputs/submission_bert.tsv`.
