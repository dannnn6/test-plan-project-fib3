# Планирование тестирования BookSphere

Лабораторная работа № 1 посвящена подготовке и сравнению тест-планов для платформы BookSphere с помощью трёх LLM. Требования к продукту приведены в [task.md](task.md). Цель - получить три итоговых документа по шаблонам IEEE 829-1998, RUP и русскому шаблону, сохранив историю подготовки и обоснование выбора.

## Навигация

- [Участники и группы](authors.md).
- [Паспорт BookSphere](task.md).
- [Студент 1 — Сунцов Р., DeepSeek](work/student1/readme.md).
- [Студент 2 — Караваев Д., ChatGPT 6](work/student2/readme.md).
- [Студент 3 — Варин Я., Claude Sonnet 5](work/student3/readme.md).
- [Сравнения, сводная таблица и итоговые планы](results/readme.md).
- [Полная структура каталогов](structura.txt).

## Исходные шаблоны

| Шаблон | Файл |
|---|---|
| IEEE 829-1998 | [TestPlanTemplate_IEEE_829-1998.pdf](standarts/TestPlanTemplate_IEEE_829-1998.pdf) |
| RUP | [TestPlanTemplate_RUP.pdf](standarts/TestPlanTemplate_RUP.pdf) |
| Русский шаблон | [Исходный DOC](standarts/План%20тестирования.doc), [PDF-копия](standarts/План%20тестирования.pdf) |

## Ход работы

1. Все участники использовали общий паспорт BookSphere и три заданных шаблона;
2. Каждый подготовил три личных тест-плана с помощью своей модели. Запросы и ответы сохранены в `work/studentN/prompt_history`, окончательные личные планы - в `work/studentN/plans`;
3. Для каждого шаблона сопоставлены три окончательные версии A/B/C. Сравнения сохранены в `results/conclusions`; таблица соответствия моделей приведена в `results/readme.md`;
4. По результатам сравнения сформированы три итоговых плана в `results/plans`;
5. При комплектовании репозитория добавлены README, список авторов, дерево и сводная таблица.

## Структура репозитория

```text
repos/
  results/
    conclusions/
      analysis_TestPlanTemplate_IEEE_829-1998.md
      analysis_plan_TestPlanTemplate_RUP.md
      analysis_plan_standart3.md
    plans/
      plan_TestPlanTemplate_IEEE_829-1998.md
      plan_TestPlanTemplate_RUP.md
      plan_План_тестирования.md
    readme.md
  standarts/
    TestPlanTemplate_IEEE_829-1998.pdf
    TestPlanTemplate_RUP.pdf
    lu259gwk.tmp
    План тестирования.doc
    План тестирования.pdf
  work/
    student1/
      plans/
        plan_TestPlanTemplate_IEEE_829-1998.md
        plan_TestPlanTemplate_RUP.md
        plan_План_тестирования.md
      prompt_history/
        prompt_history_TestPlanTemplate_IEEE_829-1998.md
        prompt_history_TestPlanTemplate_RUP.md
        prompt_history_План_тестирования.md
      readme.md
    student2/
      plans/
        plan_TestPlanTemplate_IEEE_829-1998.md
        plan_TestPlanTemplate_RUP.md
        plan_План_тестирования.md
      prompt_history/
        prompt_history_TestPlanTemplate_IEEE_829-1998.md
        prompt_history_TestPlanTemplate_RUP.md
        prompt_history_План_тестирования.md
      readme.md
    student3/
      plans/
        plan_TestPlanTemplate_IEEE_829-1998.md
        plan_TestPlanTemplate_RUP.md
        plan_План_тестирования.md
      prompt_history/
        prompt_history_TestPlanTemplate_IEEE_829-1998.md
        prompt_history_TestPlanTemplate_RUP.md
        prompt_history_План_тестирования.md
      readme.md
  authors.md
  readme.md
  structura.txt
  task.md
```

Каталог `work` хранит личные материалы; `standarts` — шаблоны; `results/conclusions` — сравнения; `results/plans` — итоговые документы. Файл `structura.txt` содержит полный перечень пользовательских файлов.
