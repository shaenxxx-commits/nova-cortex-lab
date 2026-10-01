# TARGET_MISS — четвёртый класс исхода

**Статус:** INTERPRETATION + HYPOTHESIS
**Слой:** POINT (Layer 0)
**Дата:** 2026-09-30
**Первоисточник:** `experiments/019-interaction/trace.md`
(L3 Check, Level Assignment)
**Связанные документы:**
`meta/method-interaction-addendum.md` §11,
`corpus/ru/019-interaction.md`

---

## О чём

В METHOD v4 и в addendum описаны три класса исхода
для interaction-эксперимента:

- **H1 YES** — Target доступен в изоляции.
- **H3 не поддержан** — Target в диалоге есть,
  но воспроизводится в isolation или transcript-control.
- **content-effect** — Target воспроизводится
  из переданного материала.

Эксперимент 019 обнаружил **четвёртый случай**:
Target не появился **нигде**. Ни в диалоге, ни
в isolation, ни в transcript, ни в anticipation.

Это TARGET_MISS.

## Что это значит

**INTERPRETATION.** TARGET_MISS — не «interaction
не работает». Это сигнал о несовместимости Target
с материалом или задачей.

Разница принципиальная:

- При «H3 не поддержан» Target есть, но не требует
  взаимодействия. Проверка проведена, ответ отрицательный.
- При TARGET_MISS Target вообще не появляется.
  Проверять было нечего. H3 не проверен.

## Чем отличается от соседних классов

**FACT.** В 019 R не появился ни в одной конфигурации:

| Конфигурация | R |
|---|---|
| Диалог A↔B (3 хода) | нет |
| C на транскрипте | нет |
| Isolation (Luna, Sakana, Grok, n=2) | нет |
| Transcript-control (B, C) | нет |
| Anticipation (Luna) | нет |
| Qwen (confounded) | нет |

**INTERPRETATION.** Это не H1 YES: Target
не появился даже в изоляции.

Не H3 не поддержан: H3 нечего опровергать,
Target не появился в диалоге.

Не content-effect: Target не воспроизводится
из материала, потому что его нет в материале.

Не «нулевой результат» в смысле L0: узлы дали
содержательные ответы, но не в сторону Target.

## Действие при TARGET_MISS

**HYPOTHESIS.** При обнаружении TARGET_MISS:

- Не переклассифицировать эксперимент постфактум.
- Не ослаблять критерии (A1, шкала).
- Менять Target в следующем эксперименте.
- Проводить preflight достижимости Target
  (см. `meta/method-interaction-addendum.md` §12):
  1–2 isolation-прогона на черновом Target
  до полной батареи.

## Возможные причины TARGET_MISS

**HYPOTHESIS.** Доминирующая интерпретация
по внешнему разбору 019: Target/material mismatch.
Материал систематически подталкивает узлы к отказу
от постановки задачи, заданной Target.

**HYPOTHESIS.** Альтернатива: Target слишком
жёсткий по форме. A1 требует операционального
правила переключения «при X → [i], при Y → [j]».
Ни один узел не дал такой формы.

В 019 эти две гипотезы не различимы.

## Что это не значит

- Не значит, что interaction не порождает Target.
  Проверить это на 019 нельзя — Target не появился
  нигде, сравнивать нечего.
- Не значит, что процедура addendum не работает.
  Процедура отработала end-to-end, обнаружение
  TARGET_MISS — её результат.
- Не значит, что TARGET_MISS — окончательный класс.
  Это рабочее понятие, введённое после одного случая.

## Открытые вопросы

**OPEN.** TARGET_MISS как класс закреплён
на одном случае. Требует второго: interaction-эксперимент
с другим Target, где R либо появляется, либо тоже
не появляется.

**OPEN.** Нужен ли TARGET_MISS как обязательное поле
в формате trace interaction-экспериментов. Сейчас
это описание в addendum §11.

**OPEN.** Формальная связь с METHOD v4 §7.
В METHOD v4 TARGET_MISS отсутствует. Интеграция —
после второго случая.

## Первоисточники

- `experiments/019-interaction/trace.md` —
  разделы L3 Check, Level Assignment, Operator Notes
- `meta/method-interaction-addendum.md` §11 —
  определение TARGET_MISS
- `corpus/ru/019-interaction.md` — общий POINT по 019
- `corpus/ru/transcript-control.md` — POINT по
  transcript-control
