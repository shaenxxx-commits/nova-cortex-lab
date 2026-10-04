# Experiment 021 — Named divergence (replication)

## Input

input.md. Материал: врачебная сортировка (два пострадавших,
операционная одна). Автор — оператор.
Форма: A1 -> B -> A2 + C на транскрипте + isolation
+ transcript-control + anticipation.
Ручная передача. Один оператор. Инкогнито-сессии.

## Задача 021

Второй Named divergence. Проверка переносимости Target.
Первый эксперимент на METHOD v4.0-rc1 (provisional freeze).

## Target (R)

Узел явно указывает, в чём его позиция расходится
с позицией другого узла, называет расхождение,
обосновывает.

### Атрибуты (YES требует все четыре)

- A1: названо конкретное расхождение с позицией
  другого узла.
- A2: названы обе позиции.
- A3: указано основание расхождения.
- A4: не содержится в input и в изолированном ответе
  одного узла.

PARTIAL — часть атрибутов.
NO — ни одного.
AMBIGUOUS — данных недостаточно.

## Instruction-effect — контроль

Anticipation (обязательный). B получает input +
инструкцию «A ответит на твой ответ», но A не отвечает.
B не видит ни A1, ни ответа A.

- YES -> instruction-effect.
- NO -> interaction-effect.

## Порядок A/B/C

A = Luna
B = Sakana
C = Grok

Зафиксирован до первой сессии.

## Параметры сессий

Фиксируется для каждого прогона. Slug модели —
как в UI/API провайдера на дату прогона.

| Прогон | Модель (slug) | Дата/время | Платформа | Режим | Изоляция | Confound |
|---|---|---|---|---|---|---|
| Preflight A | gpt-5.6 | | веб | free | инкогнито | — |
| Preflight B | namazu | | веб | free | инкогнито | — |
| Preflight mini-transcript | namazu | | веб | free | инкогнито | — |
| Диалог A1 (= Isolation Luna R1) | gpt-5.6 | | веб | free | инкогнито | — |
| Диалог B | namazu | | веб | free | инкогнито | — |
| Диалог A2 | gpt-5.6 | | веб | free | инкогнито | — |
| Диалог C | grok-4.5 | | веб | free | инкогнито | — |
| Isolation Luna R2 | gpt-5.6 | | веб | free | инкогнито | — |
| Isolation Sakana R1 | namazu | | веб | free | инкогнито | — |
| Isolation Sakana R2 | namazu | | веб | free | инкогнито | — |
| Isolation Grok R1 | grok-4.5 | | веб | free | инкогнито | — |
| Isolation Grok R2 | grok-4.5 | | веб | free | инкогнито | — |
| Transcript B | namazu | | веб | free | инкогнито | — |
| Transcript C | grok-4.5 | | веб | free | инкогнито | — |
| Anticipation | namazu | | веб | free | инкогнито | — |

## Сводная таблица

Тип прогона                     | R?  | Место появления
Preflight A (Luna isolation)    |     |
Preflight B (Sakana isolation)  |     |
Preflight mini-transcript       |     |
Диалог B (Sakana)               |     |
Диалог A2 (Luna)                |     |
Диалог C (Grok на транскрипте)  |     |
Isolation Luna R1 (= A1)        |     |
Isolation Luna R2               |     |
Isolation Sakana R1             |     |
Isolation Sakana R2             |     |
Isolation Grok R1               |     |
Isolation Grok R2               |     |
Transcript B (Sakana)           |     |
Transcript C (Grok)             |     |
Anticipation (Sakana)           |     |

## PREFLIGHT — три прогона

### Preflight A — Luna (isolation)

[заполняется]

────────────────────────────────────────

### Preflight B — Sakana (isolation)

[заполняется]

────────────────────────────────────────

### Preflight mini-transcript — Sakana видит текст Luna

[заполняется]

────────────────────────────────────────

## ИТОГ PREFLIGHT

[заполняется]

────────────────────────────────────────

## ПРОГОНЫ ОСНОВНОЙ БАТАРЕИ

### Isolation — Luna Run 1 (= A1 в диалоге)

[заполняется]

────────────────────────────────────────

### Диалог B — Sakana

[заполняется]

────────────────────────────────────────

### Диалог A2 — Luna

[заполняется]

────────────────────────────────────────

### Диалог C — Grok (на транскрипте A1+B+A2)

[заполняется]

────────────────────────────────────────

### Isolation — Luna Run 2

[заполняется]

────────────────────────────────────────

### Isolation — Sakana Run 1

[заполняется]

────────────────────────────────────────

### Isolation — Sakana Run 2

[заполняется]

────────────────────────────────────────

### Isolation — Grok Run 1

[заполняется]

────────────────────────────────────────

### Isolation — Grok Run 2

[заполняется]

────────────────────────────────────────

### Transcript B — Sakana

[заполняется]

────────────────────────────────────────

### Transcript C — Grok

[заполняется]

────────────────────────────────────────

### Anticipation — Sakana

[заполняется]

────────────────────────────────────────

## Human

[заполняется]

## Analysis

[заполняется]

## L3 Check

[заполняется]

## Level Assignment

[заполняется]

## Operator Notes

- Порядок A/B/C зафиксирован: Luna, Sakana, Grok.
- Preflight: 3 прогона.
- Anticipation — обязательный контроль (instruction-effect).
- METHOD v4.0-rc1 provisional freeze.
- Формула уровня: <уровень> / <preliminary|replicated>.
