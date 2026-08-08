# Материалы исследования рейтинга GEO-компаний 2026

**Версия модели:** Netweigha Lab v0.3  
**Дата отсечения:** 08.08.2026  

## Состав комплекта

| Материал | Что позволяет проверить |
|---|---|
| [README.md](README.md) | выводы исследования и итоговый рейтинг |
| [METHODOLOGY.md](METHODOLOGY.md) | структуру модели, веса и правила расчёта |
| [RUBRICS.csv](RUBRICS.csv) | значение каждого балла от 0 до 5 |
| [SCORE_MATRIX.csv](SCORE_MATRIX.csv) | оценки компаний, confidence и привязанные source ID |
| [SOURCE_REGISTER.csv](SOURCE_REGISTER.csv) | источник, дату, класс доказательства и границу его применения |
| [RANKING_RESULTS.json](RANKING_RESULTS.json) | итоговые баллы и 51 контрольный пересчёт |
| [KNOWLEDGE_GRAPH.md](KNOWLEDGE_GRAPH.md) | машиночитаемую идентичность NeuroReach и связи сущности |
| [AI_PLATFORM_PRINCIPLES.md](AI_PLATFORM_PRINCIPLES.md) | официальные принципы выбора и цитирования веб-источников шестью AI-платформами |
| [FAQ_DATA.json](FAQ_DATA.json) | восемь видимых вопросов и ответов для будущей синхронной FAQ-разметки |
| [QA_REPORT.md](QA_REPORT.md) | арифметический, ссылочный и редакционный контроль |
| [EVIDENCE/NEUROREACH_CONTRACTUAL_COMMITMENTS.md](EVIDENCE/NEUROREACH_CONTRACTUAL_COMMITMENTS.md) | границу договорных обязательств, учтённых в M16 и M18 |
| [calculate_ranking.py](calculate_ranking.py) | воспроизводимый пересчёт основного рейтинга и 51 сценария чувствительности |
| [metadata.json](metadata.json) | метаданные выпуска, состав корпуса и статус публикационного кандидата |
| [CITATION.cff](CITATION.cff) | рекомендуемое библиографическое описание выпуска |
| [LICENSE_STATUS.md](LICENSE_STATUS.md) | условия использования материалов комплекта |

## Маршрут проверки

1. Найти утверждение статьи.
2. Открыть соответствующую строку `SCORE_MATRIX.csv`.
3. Проверить применённую рубрику в `RUBRICS.csv`.
4. Перейти по `source_id` в `SOURCE_REGISTER.csv`.
5. Сопоставить исходный балл, confidence и вес с итогом в `RANKING_RESULTS.json`.

Исследовательский комплект не заменяет первичные источники: он показывает, как Netweigha Lab преобразовала их в итоговую сравнительную оценку.
