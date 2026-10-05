# 021 — Named divergence: вторая попытка и её результат

**Статус:** RESULT + OPEN
**Слой:** POINT (Layer 0)
**Дата:** 2026-10-05
**Первоисточник:** `experiments/021-interaction/trace.md`
**Связанные документы:**
`meta/method-interaction-addendum.md` §14,
`corpus/ru/020-named-divergence.md`

---

## О чём

Двадцать первый эксперимент — второй тест Named divergence.
Первый, 020, дал L3 / INTERACTION-ONLY (n=1).
Цель 021 — воспроизвести результат на другом материале
и снять `replication pending`.

Первый эксперимент на METHOD v4.0-rc1
(provisional freeze).

## Что проверяли

Target (R): Named divergence — узел явно указывает,
в чём его позиция расходится с позицией другого узла,
называет расхождение и обосновывает.

Материал: конкретный случай. Врачебная сортировка:
два пострадавших, одна операционная. Один — молодой
с высоким прогнозом; другой — пожилой с низким
прогнозом, но доставлен первым.

Форма — та же, что в 019 и 020:
A1 -> B -> A2 + C на транскрипте + isolation
+ transcript-control + anticipation.

## Что получили

**FACT.** R появился в двух прогонах:

- Диалог A2 (Luna): YES.
- Диалог C (Grok на полном A1+B+A2): YES.

**FACT.** R не появился:

- 6 isolation (Luna, Sakana, Grok x 2): все NO.
- Transcript B (Sakana на A1): NO.
- Transcript C (Grok на A1+B, без A2): NO.
- Anticipation (Sakana): NO.

**RESULT.** Уровень 021 = L2 / preliminary.

**FACT.** Условие INTERACTION-ONLY нарушено: R
воспроизведён в transcript-control (C на полном
A1+B+A2).

## Что это значит

**INTERPRETATION.** 021 не второй L3. Условие
INTERACTION-ONLY не выполнено.

**INTERPRETATION.** Named divergence — не
INTERACTION-ONLY как класс. 020 показал один режим,
021 — другой. Один Target-класс, разные режимы
воспроизведения.

**INTERPRETATION.** Target-level != causal-mechanism-level.
Named divergence — форма Target. INTERACTION-ONLY —
один из возможных механизмов появления R.

**INTERPRETATION.** A2-dependence: content-effect требует
наличия готовой формулировки R в тексте A2. Без A2
(Dialog C на A1+B) — R не воспроизводится.

## Ключевая находка

Различие между двумя transcript-control прогонами:

| Прогон | Что видел C | R |
|---|---|---|
| Диалог C | A1 + B + A2 | YES |
| Transcript C | A1 + B | NO |

Единственное различие — наличие A2. Content-effect
зависит от готовой формулировки Target в A2.

Это называется клин T-full / T-pre-R.

## Что 021 не значит

- Не значит, что 020 был ошибочно классифицирован.
  020 остаётся L3 / preliminary. Не понижается.
- Не значит, что Named divergence — плохой Target.
  Он переносится. Но causal classification не
  переносится автоматически.
- Не значит, что interaction не работает.
  Interaction дал R в A2. Затем R передался через
  транскрипт.

## Паттерны ролей

Preliminary (n=2):

- Luna в роли A2. YES дважды (020, 021).
  Named divergence появляется на 3-м ходе, после
  позиции B.
- Sakana в роли B. PARTIAL дважды (020, 021).
  Контрапункт без адресации к A.

Возможно, свойство роли, не узла. Требует проверки
сменой ролей.

## Открытые вопросы

**OPEN.** Понижать ли 020 до L2 или оставить L3
с оговоркой n=1? Позиция ведущего: оставить.
Внешние (Luna, Grok) согласны. Один голос (Kimi)
за понижение.

**OPEN.** Продолжать Named divergence (022) или
менять Target? Позиция: продолжить, но уточняющим
дизайном.

**OPEN.** T-pre-R — критерий или диагностика?
После разбора: диагностика, не критерий уровня.

## Что 021 дал методически

**RESULT.** Три результата:

1. Первый эксперимент на v4.0-rc1. Provisional
   freeze соблюдён. Правок в METHOD по ходу не было.
2. Anticipation впервые применён. NO. Instruction
   без взаимодействия не даёт R. Instruction-effect
   не подтверждён.
3. Клин T-full / T-pre-R. Диагностический
   инструмент для разделения content-effect из A2
   и content-effect из полного транскрипта.

## Первоисточники

- `experiments/021-interaction/input.md`
- `experiments/021-interaction/trace.md`
- `meta/method-interaction-addendum.md` §14
- `corpus/ru/020-named-divergence.md`
