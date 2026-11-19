# Домашнее задание: агенты и их тестирование

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nikis14/llm-course-hw-agents-evals/blob/main/hw_agents_evals.ipynb)

HR-ассистент компании «Полярис»: строим eval-пайплайн (кодовые грейдеры, LLM-as-a-judge с калибровкой по каппе Коэна), пишем ReAct-агента на чистом Python и на LangGraph, проектируем собственные инструменты и оцениваем траектории агента.

## Как начать

1. Откройте ноутбук в Colab по кнопке выше.
2. **File → Save a copy in Drive** — работайте в своей копии.
3. Выполняйте ячейки сверху вниз. Данные ноутбук скачает сам из папки `hw_data/` этого репозитория.

Понадобится API-ключ Neural Deep (или другого OpenAI-совместимого провайдера с поддержкой tool calling — см. `PROVIDERS` в ноутбуке).

## Что в репозитории

| Файл | Что это |
|---|---|
| `hw_agents_evals.ipynb` | ноутбук с заданием |
| `hw_data/hr_db.json` | мок HR-системы: сотрудники, остатки отпусков, больничные, календарь команд, заявки |
| `hw_data/policies.json` | внутренние политики компании и страницы вики |
| `hw_data/eval_set.json` | eval-набор из 20 задач |
| `hw_data/judge_calibration.json` | 44 ответа ассистента с разметкой двух ассесоров — для калибровки judge |
| `hw_data/recorded_traces.json` | 18 трейсов старой версии агента с эталонными метками — для проверки грейдеров траектории |
| `hw_data/skills/` | шаблон `SKILL.md` и заготовка скилла |

Все данные синтетические.
