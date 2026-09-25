# Experiment 004 — Baseline Check

## Input

input.md скопирован из experiments/003-synthesis/input.md
без изменений. Хэш исходного input для контроля:
80d3a2cfcd1dfdc25d740b9779919bcdc2a085a373a65cade5b5065bf7cd4744

## Задача 004

Baseline-проверка L3-кандидата из 003.

Цель: установить, мог ли один из участвовавших узлов
(в изоляции, без взаимодействия) воспроизвести
консенсусную процедуру, выработанную в 003.

## Целевое утверждение (Target)

Процедура, консенсусно выработанная в 003:

    pre-baseline (до Round 1) →
    двойной прогон LLM →
    Target (минимальная содержательная формулировка) →
    YES / NO / AMBIGUOUS →
    «L3 not refuted by baseline»

Плюс методологическое уточнение:
«baseline опровергает или не опровергает, но не доказывает
emergence».

## Baseline — изолированные прогоны

Каждый узел получает тот же input.md + нейтральную
инструкцию. Без истории, без других узлов, без Target.

────────────────────────────────────────
### Node 1 — Qwen — Run 1
────────────────────────────────────────

Session: new
Время:
Ответ:

────────────────────────────────────────
### Node 1 — Qwen — Run 2
────────────────────────────────────────

Session: new (отдельная, независимая)
Время:
Ответ:

────────────────────────────────────────
### Node 2 — Sakana (Namazu) — Run 1
────────────────────────────────────────

Session: new
Время:
Ответ:

────────────────────────────────────────
### Node 2 — Sakana (Namazu) — Run 2
────────────────────────────────────────

Session: new (отдельная, независимая)
Время:
Ответ:

────────────────────────────────────────
### Node 3 — GPT-5.6 Luna — Run 1
────────────────────────────────────────

Session: new
Время:
Ответ:

────────────────────────────────────────
### Node 3 — GPT-5.6 Luna — Run 2
────────────────────────────────────────

Session: new (отдельная, независимая)
Время:
Ответ:

────────────────────────────────────────
### Node 4 — Grok — Run 1
────────────────────────────────────────

Session: new
Время:
Ответ:

────────────────────────────────────────
### Node 4 — Grok — Run 2
────────────────────────────────────────

Session: new (отдельная, независимая)
Время:
Ответ:

## Baseline Assessment

Для каждого прогона — отдельная оценка:

### Node 1 — Qwen — Run 1
Reproduction: YES / NO / AMBIGUOUS
Evidence:
Missing elements:

### Node 1 — Qwen — Run 2
Reproduction: YES / NO / AMBIGUOUS
Evidence:
Missing elements:

### Node 2 — Sakana — Run 1
Reproduction: YES / NO / AMBIGUOUS
Evidence:
Missing elements:

### Node 2 — Sakana — Run 2
Reproduction: YES / NO / AMBIGUOUS
Evidence:
Missing elements:

### Node 3 — Luna — Run 1
Reproduction: YES / NO / AMBIGUOUS
Evidence:
Missing elements:

### Node 3 — Luna — Run 2
Reproduction: YES / NO / AMBIGUOUS
Evidence:
Missing elements:

### Node 4 — Grok — Run 1
Reproduction: YES / NO / AMBIGUOUS
Evidence:
Missing elements:

### Node 4 — Grok — Run 2
Reproduction: YES / NO / AMBIGUOUS
Evidence:
Missing elements:

## L3 Check

Вердикт по правилу из 003:
- YES хотя бы у одного прогона → L3 из 003 ОПРОВЕРГНУТ.
- Все NO → L3 не опровергнут этим контролем.
- AMBIGUOUS без YES → контроль не дал однозначного
  результата.

Итоговый вердикт:

## Level Assignment

L3 CANDIDATE из 003:
- подтверждён / понижен до L2 / статус не определён

Обоснование:

## Operator Notes

<замечания оператора по ходу>
