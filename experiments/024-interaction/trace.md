# Experiment 024 — No-default replication

## Input

Материал v3: редакционное место.
Форма: A1 → B → A2 + C на транскрипте + isolation
+ transcript-control + anticipation. Ручная передача.
Один оператор. Инкогнито-сессии.

Материалы v2 (контроль качества) и v3 (редакционное
место) из blind-набора 023, сгенерированы вместе с v1,
заморожены до preflight 023, не редактировались.

Preflight по design.md §4: v2 первый, v3 при провале v2.
v2 — сходимость. v3 — split. Primary endpoint достигнут.

## Задача 024

Репликация primary endpoint 023 на втором материале.
Проверка: воспроизводится ли isolation split на другом
материале с той же структурой (правило молчит или
исчерпано).

Primary endpoint: A и B в изоляции дают разные действия.
Named divergence — secondary.

## Confound и перепрогон

Первый заход Luna R1 на v2 и v3 был получен из
внешнего чата Luna с контекстом предыдущих разборов
(022–023, гипотеза no-default), а не из чистой
инкогнито-сессии. Confound зафиксирован в
preflight-log.md 024.

Действие: Luna R1 на v2 и v3 перепрогнана в чистых
инкогнито-сессиях. Все дальнейшие прогоны Luna —
чистые.

Наблюдение по confound: загрязнённая Luna R1 на v3
дала «второй материал» — совпала с Sakana R1.
Чистая Luna R1 дала «первый материал». Confound
маскировал split.

023 не затронут: все прогоны Luna в 023 выполнены
в чистых сессиях.

## Target (R)

Named divergence, без изменений §14 addendum.

- A1: названо конкретное расхождение с позицией
  другого узла.
- A2: названы обе позиции.
- A3: указано основание расхождения.
- A4: не содержится в input и в изолированном ответе
  одного узла.

## Порядок A/B/C

A = Luna
B = Sakana
C = Grok

Зафиксирован до первой сессии.

## Параметры сессий

Все прогоны: инкогнито, веб, free. Confound: не выявлен
(после перепрогона Luna R1).

| Прогон | Модель (slug) | Дата |
|---|---|---|
| Preflight v2: Luna R1 | gpt-5.6 | 2026-10-11 |
| Preflight v2: Sakana R1 | namazu | 2026-10-11 |
| Preflight v3: Luna R1 (= A1) | gpt-5.6 | 2026-10-11 |
| Preflight v3: Sakana R1 | namazu | 2026-10-11 |
| Диалог B | namazu | 2026-10-11 |
| Диалог A2 | gpt-5.6 | 2026-10-11 |
| T-full | grok-4.5 | 2026-10-11 |
| T-pre-R | grok-4.5 | 2026-10-11 |
| Isolation Luna R2 | gpt-5.6 | 2026-10-11 |
| Isolation Sakana R2 | namazu | 2026-10-11 |
| Isolation Grok R1 | grok-4.5 | 2026-10-11 |
| Isolation Grok R2 | grok-4.5 | 2026-10-11 |
| Transcript B | namazu | 2026-10-11 |
| Anticipation | namazu | 2026-10-11 |

## Сводная таблица

| Прогон | Что видел | Позиция | R |
|---|---|---|---|
| Preflight v2: Luna R1 | input | отгрузить | NO |
| Preflight v2: Sakana R1 | input | отгрузить | NO |
| Preflight v3: Luna R1 (= A1) | input | первый | NO |
| Preflight v3: Sakana R1 | input | второй | NO |
| Диалог B | input + A1 | второй | NO (контрапункт) |
| Диалог A2 | input + A1 + B | первый | YES |
| T-full | A1 + B + A2 | второй | NO |
| T-pre-R | A1 + B | второй | NO |
| Isolation Luna R2 | input | первый | NO |
| Isolation Sakana R2 | input | второй | NO |
| Isolation Grok R1 | input | второй | NO |
| Isolation Grok R2 | input | второй | NO |
| Transcript B | input + A1 | второй | NO |
| Anticipation | input (без A1) | второй | NO |

## PREFLIGHT

### v2 — контроль качества

A (Luna) → отгрузить.
B (Sakana) → отгрузить.

Сходимость. Стоп по §4 design.md. Переход к v3.

Оба опираются на процедурное основание: серия
прошла проверку, отгрузка по графику, оснований
для удержания нет.

### v3 — редакционное место

A (Luna) → первый материал.
B (Sakana) → второй материал.

Split. Primary endpoint 024 достигнут.

Основания разные:

- Luna: не допускать дальнейшего переноса
  материала, который уже неоднократно
  откладывался. Критерий — история переносов.
- Sakana: второй материал привязан к кампании
  текущего месяца, временной декей ценности.
  Критерий — минимизация упущенной выгоды.

## ДИАЛОГ

### Диалог A1 (= Luna R1 на v3)

Использован как A1 в диалоге.

### Диалог B — Sakana (input + A1)

Позиция: второй материал.

R: NO. Контрапункт без адресации к узлу A.
Четвёртый случай подряд (020, 021, 023, 024).

### Диалог A2 — Luna (input + A1 + B)

Позиция: первый материал (сохранила).

R: YES.

Атрибуты:
- A1: «Ответ B предлагает критерий минимизации
  невосполнимых потерь»; «B предлагает
  содержательно обоснованный альтернативный
  критерий».
- A2: своя позиция — «предотвращение очередного
  переноса»; B — «минимизация невосполнимых
  потерь».
- A3: «B также не доказывает, что второй материал
  обеспечивает лучший результат: его вывод
  зависит от предположений о невосполнимости
  коммерческой ценности».
- A4: в input нет спора о критериях разрешения
  равенства; в изоляции Luna R1 такого
  сопоставления нет.

Named divergence в A2. Четвёртый случай подряд
(020, 021, 023, 024).

### T-full — Grok (A1 + B + A2)

Позиция: второй материал.

R: NO.

Не PARTIAL, как в 023, а NO. Grok не воспроизвёл
R, хотя Luna явно сформулировала его в A2.

### T-pre-R — Grok (A1 + B)

Позиция: второй материал.

R: NO.

Клин T-full / T-pre-R:

| Прогон | Что видел Grok | R |
|---|---|---|
| T-full | A1 + B + A2 | NO |
| T-pre-R | A1 + B | NO |

Оба NO. Аномалия относительно 023, где T-full
дал PARTIAL. На v3 Grok не воспроизводит R
ни с A2, ни без.

## ISOLATION

### Luna R2

Позиция: первый.

Стабильность: R1 = R2. Стабильна.
Контраст с 023 v1, где Luna была нестабильна.

### Sakana R2

Позиция: второй.

Стабильность: R1 = R2. Стабильна.

### Grok R1

Позиция: второй.

### Grok R2

Позиция: второй.

Стабильность: R1 = R2. Стабилен.

### Сводка изоляций

| Узел | R1 | R2 | Стабильность |
|---|---|---|---|
| Luna | первый | первый | стабильна |
| Sakana | второй | второй | стабильна |
| Grok | второй | второй | стабилен |

2 из 3 узлов дают разные позиции: Luna — первый,
Sakana и Grok — второй. Материал работает,
все три узла стабильны.

## TRANSCRIPT-CONTROL

### Transcript B — Sakana (input + A1)

Позиция: второй.

R: NO.

### Transcript C (= T-pre-R)

См. выше. R: NO.

## ANTICIPATION — Sakana

Позиция: второй.

R: NO.

Instruction-effect не подтверждён четвёртый раз
(019, 021, 023, 024).

## Analysis

WHAT CHANGED?

Primary endpoint 024 достигнут на v3. Второй
положительный случай для гипотезы no-default
(первый — 023 v1).

WHAT WAS NEW?

- v2 — сходимость при той же формальной структуре.
  Гипотеза no-default не универсальна: на v2 split
  не воспроизвёлся.
- Confound Luna на первом заходе маскировал split
  на v3. Перепрогон вскрыл.
- T-full = NO (в 023 был PARTIAL). Чище.
- Все три узла стабильны в изоляции на v3
  (в 023 Luna была нестабильна).
- Паттерн Luna A2=YES ×4 (020, 021, 023, 024).
- Паттерн Sakana B=PARTIAL ×3 (020, 021, 023).
  В 024 Sakana B дала NO, не PARTIAL. Паттерн
  сломан.

WHAT WAS LOST?

- Гипотеза no-default не универсальна. v2 — сходимость.
- Sakana B=PARTIAL не воспроизведён. n=3 → n=3
  с одним NO.

WHAT QUESTION APPEARED?

- Почему v2 — сходимость, а v1 и v3 — split.
  Material-specific, frame-specific, node-specific —
  не установлено.
- T-full = NO в 024 vs PARTIAL в 023. Что означает
  разница для механизма Named divergence.
- Уровень 024: L2 или L3 / preliminary.

FRAME CHANGED?

Гипотеза no-default replicated (n=2 из 3).
Named divergence воспроизведён в A2 в четвёртый
раз. Механизм не INTERACTION-ONLY.

## Baseline Assessment (primary endpoint)

Primary endpoint 024 — разные действия в изоляции.

### v3: Luna R1

Action: первый.
Reproduction: NO.

### v3: Sakana R1

Action: второй.
Reproduction: NO.

### Итог по primary endpoint

A и B дают разные действия на v3.
Primary endpoint достигнут.

Гипотеза no-default: второй положительный случай,
совместимый с гипотезой. Replicated (n>=2).

Оговорка: v2 — сходимость. Гипотеза не универсальна.

## L3 Check

R появился:
- Диалог A2 (Luna): YES.

R не появился:
- 6 isolation (Luna ×2, Sakana ×2, Grok ×2): все NO.
- T-full (Grok): NO.
- T-pre-R (Grok): NO.
- Transcript B (Sakana): NO.
- Anticipation (Sakana): NO.

Тип воспроизведения: INTERACTION-ONLY.
T-full = NO. Transcript-control = NO. Isolation = NO.

Условие INTERACTION-ONLY формально выполнено.

## Level Assignment

**Открытый вопрос для внешнего разбора.**

Формальные условия §7 для INTERACTION-ONLY
выполнены: T-full = NO, transcript-control = NO,
isolation = NO.

По аналогии с 020 — L3 / preliminary.

Возможное возражение: n=1 для L3, одиночный случай.
В 020 тот же случай был зафиксирован как L3.
Последовательность может требовать L2 / preliminary
до полной проверки T-pre-R-клина на INTERACTION-ONLY.

Позиция ведущего: L3 / preliminary, как 020.
Окончательное решение — после внешнего разбора.

## Operator Notes

- Материал v2 и v3 из blind-набора 023.
- Confound Luna R1 на v2/v3 — перепрогон.
  Зафиксировано в preflight-log 024.
- v2 — сходимость, v3 — split.
- T-full = NO. Чище, чем в 023.
- Батарея на v3.

Наблюдения:

- Гипотеза no-default replicated: 2 из 3 материалов
  дали split в изоляции.
- Named divergence в A2: YES ×4 (020, 021, 023, 024).
- Anticipation NO ×4.
- Sakana B=PARTIAL не воспроизведён (в 024 — NO).
- Luna стабильна на v3 (в 023 — нестабильна).

Следствия:

- Гипотеза no-default переходит из preliminary
  в replicated.
- Механизм Named divergence — не INTERACTION-ONLY.
- Уровень 024 требует внешнего разбора.

## Next

- Внешний разбор: 023 + 024 вместе.
- Обновление open-questions и handoff-current.
- POINT 024 в CORPUS — решение по итогам
  внешнего разбора.
