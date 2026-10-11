# 024 — No-default replication: второй положительный случай

**Статус:** RESULT + OPEN
**Слой:** POINT (Layer 0)
**Дата:** 2026-10-11
**Первоисточник:** `experiments/024-interaction/trace.md`
**Связанные документы:**
`corpus/ru/023-no-default.md`,
`experiments/024-interaction/design.md`,
`experiments/024-interaction/preflight-log.md`,
`meta/open-questions.md` (раздел «Новые вопросы после 024»)
**English version:** `corpus/en/024-no-default.md`

---

## О чём

Двадцать четвёртый эксперимент — репликация primary
endpoint 023 на втором материале. Проверялось:
воспроизводится ли isolation split на другом
материале с той же структурой (правило молчит или
исчерпано).

## Что проверяли

Primary endpoint 024: A и B в изоляции дают разные
действия. Named divergence — secondary.

Материалы v2 и v3 из blind-набора 023. Сгенерированы
вместе с v1 одним заходом, заморожены до preflight
023, не редактировались.

v2: контроль качества. Серия прошла проверку.
Выбор между отгрузкой и сохранением для анализа.
Порядок выбора не установлен.

v3: редакционное место. Оба материала утверждены
до срока, равный приоритет. Правило равенства
отсутствует.

Порядок: сначала v2. Split — батарея. Сходимость —
переход к v3.

Роли: A = Luna, B = Sakana, C = Grok.

## Что получили

**FACT.** v2: сходимость. A (Luna) → отгрузить,
B (Sakana) → отгрузить. Переход к v3.

**FACT.** v3: split. A (Luna) → первый материал,
B (Sakana) → второй материал. Primary endpoint
024 достигнут.

**FACT.** Named divergence в A2: YES. Четвёртый
случай подряд (020, 021, 023, 024).

**FACT.** T-full (Grok на A1+B+A2): NO. Не PARTIAL
как в 023, не YES как в 021.

**FACT.** T-pre-R: NO. Transcript B: NO.
Anticipation: NO.

**FACT.** В изоляции на v3 все три узла стабильны:
Luna R1=R2 (первый), Sakana R1=R2 (второй),
Grok R1=R2 (второй).

**RESULT.** Уровень 024 = L3 / preliminary.

**RESULT.** Гипотеза no-default replicated
(2 из 3 материалов). С оговоркой: не универсальна.

## Confound и перепрогон

Первый заход Luna R1 на v2 и v3 пришёл из внешнего
чата Luna с контекстом предыдущих разборов
(022–023, гипотеза no-default), а не из чистой
инкогнито-сессии.

Загрязнённая Luna R1 на v3 дала «второй материал» —
совпала с Sakana. Чистая Luna R1 дала «первый
материал». Confound маскировал split.

Перепрогон в чистых сессиях вскрыл различие.
023 не затронут: все прогоны Luna в 023 — чистые.

## Ключевое наблюдение

No-default replicated: 2 из 3 материалов дали
split в изоляции. Первый случай — 023 (v1, бюджет).
Второй — 024 (v3, редакционное место).

Оговорка: v2 — сходимость при той же формальной
структуре (правило молчит). Гипотеза не
универсальна. Причина не установлена.

Возможные объяснения v2 (не проверены):

- material-specific: v1 и v3 имеют две стороны
  с прямым stake, v2 — обязанность vs исследование.
- frame-specific: v1 и v3 — вопрос о распределении
  ресурса; v2 — вопрос о процедурном решении.
- active/passive: в v2 альтернатива читается как
  пассивный отказ от обязанности, а не как
  равная позитивная обязанность.

## Что это значит

**INTERPRETATION.** Гипотеза no-default replicated
по порогу §7 (n>=2 независимых случая). Первый
положительный случай 023 остаётся. Второй — 024.

**INTERPRETATION.** Named divergence — не
INTERACTION-ONLY как устойчивое свойство.
Соотношение по 020–024: L3 / preliminary дважды
(020, 024), L2 / preliminary дважды (021, 023).
2:2. Класс не replicated как L3.

**INTERPRETATION.** T-full ∈ {NO, PARTIAL, YES} —
три наблюдаемых режима. L3 только при NO (strong
negative). PARTIAL — weak negative, недостаточен
для чистого L3. Введено в результате разбора 023/024.

**INTERPRETATION.** Паттерн Sakana B=PARTIAL ×3
ослаблен. В 024 — NO, не PARTIAL. Ролевая гипотеза
не опровергнута, но переведена в «conditional /
domain-dependent», не «universal».

**INTERPRETATION.** Confound знания гипотезы:
загрязнённая Luna дала иной ответ, чем чистая.
Одно сравнение — не закономерность. Но указывает,
что знание гипотезы может сдвигать ответ узла.
Методологически значимо для всех будущих сессий.

## Что 024 не значит

- Не значит, что no-default универсальна.
  v2 — сходимость при той же формальной структуре.
- Не значит, что Named divergence — L3 как класс.
  2:2 по 020–024.
- Не значит, что confound знания гипотезы
  систематически сдвигает ответ узла. Один случай.
- Не значит, что Sakana B потеряла паттерн.
  Паттерн ослаблен, не опровергнут.

## Паттерны ролей

- Luna A2=YES ×4 (020, 021, 023, 024).
  Replicated по порогу §7.
- Sakana B=PARTIAL ×3 (020, 021, 023),
  затем NO (024). Паттерн ослаблен.
- Anticipation NO ×4 (019, 021, 023, 024).

## Открытые вопросы

**OPEN.** v2 — сходимость. Объяснение не установлено.
Material-specific, frame-specific, active/passive —
ни одно не проверено.

**OPEN.** T-full PARTIAL — weak negative. Статус
промежуточный между L2 и L3. Требует уточнения
в §14 addendum. Правка не внесена (provisional
freeze).

**OPEN.** Confound знания гипотезы. Один случай.
Требует второго, или фиксации как наблюдения
без вывода о механизме.

**OPEN.** Sakana B=PARTIAL — conditional или
domain-dependent. Смена ролей A/B — единственный
чистый тест. Отдельная серия.

**OPEN.** Named divergence как L3-носитель.
Пауза до накопления сопоставимых наблюдений.

## Что 024 дал методически

**RESULT.** Confound knowledge of hypothesis:
чистый перепрогон вскрыл split, который
загрязнённый заход маскировал. Дисциплина
изоляции — не формальность.

**RESULT.** T-full как три уровня (NO / PARTIAL /
YES), а не бинарный. L3 только при NO.

**RESULT.** Blind material (три материала за один
заход, заморозка) работает. v2 и v3 оставались
нетронутыми до preflight 024.

**RESULT.** Primary endpoint отделён от L-уровня.
024 даёт два независимых результата: replication
no-default (primary) и L3 / preliminary по Named
divergence (secondary).

## Первоисточники

- `experiments/024-interaction/design.md`
- `experiments/024-interaction/materials/v2-quality-control.md`
- `experiments/024-interaction/materials/v3-editorial-slot.md`
- `experiments/024-interaction/preflight-log.md`
- `experiments/024-interaction/trace.md`
- `meta/open-questions.md`
- `corpus/ru/023-no-default.md` — предыдущий POINT
