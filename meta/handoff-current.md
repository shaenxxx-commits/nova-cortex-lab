# HANDOFF CURRENT

**Дата:** 2026-10-04
**Статус:** актуальный

Снимок текущего состояния LAB. Передаётся новому
ведущему при смене чата. Проверяется по §8
handoff-protocol.

## HEAD

- LAB: e7db91e (main-working = origin/main)
- blog: 761cb9e (main)

## Что сделано в сессии

Сессия: 2026-10-03 — 2026-10-04.

- 019 закрыт. TARGET_MISS, L1.
- 020 закрыт. L3 / INTERACTION-ONLY, n=1.
  Первый положительный H3-тест. Target —
  Named divergence.
- CORPUS v0 собран: 3 POINT (019-interaction,
  transcript-control, target-miss) + SEQUENCE
  019-trajectory. Плюс POINT 020-named-divergence.
- X-аккаунт создан (@Shaen___). Два поста: 019, 020.
- Blog на GitHub Pages: 5 постов.
- Addendum обновлён: §14 Named divergence,
  §12 Preflight, §10 статус после 020.
- Разбор Z (2026-10-03). Группа A исправлений:
  - PARTICIPANTS: mapping псевдоним → модель.
  - METHOD §5.4: обязательные параметры сессий.
  - METHOD §7: пороги n для типов выводов.
  - trace 009, 011, 019, 020: таблицы параметров.
  - provenance: дополнен 014–020.
  - ontology-log: v2 + v2.1.
- Внешние: Luna и Grok разобрали 020.
  Z — разовый структурный разбор.
- Группа A+ (после разбора Luna, Grok, Kimi):
  - PARTICIPANTS: DeepSeek — ведущий, не узел;
    LAB-наблюдения для Luna/Sakana/Grok/Qwen;
    Kimi — веб-чат OpenRouter (не CLI).
  - METHOD: пометка amendments; уточнение slug;
    уточнение replicated (replication threshold,
    не статистический порог); §5.1 -> §5.3.
  - Kimi — третий постоянный внешний, ответ получен.
  - Промежуточный прогон группы A через Luna, Grok, Kimi
    сделан.
- 021 закрыт. Named divergence, второй случай.
  L2 / preliminary. INTERACTION-ONLY не replicated.
- Ключевая находка 021: T-full / T-pre-R wedge.
  Content-effect зависит от A2.
- §14 addendum: substantive amendment после 021.
- POINT 021 в CORPUS (ru + en).
- Паттерны ролей: Luna A2=YES x2, Sakana B=PARTIAL x2.

## Внешние системы

- X: @Shaen___. Три поста: 019, 020, 021.
  Активность нулевая. Публикуется как фиксация,
  не для охвата.
- blog: https://shaenxxx-commits.github.io
  Posts: /019-trajectory/, /019-interaction/,
  /transcript-control/, /target-miss/,
  /020-named-divergence/, /021-named-divergence/.
- GitHub Pages: активен.
- CORPUS: публикационный слой в corpus/.
  ru/ + en/ + publications/.

## Ограничения и предпочтения

См. `meta/operator-preferences.md`.

## Где смотреть

- `meta/context.md` — стратегический контекст
  (MAIA / LAB / CORPUS).
- `meta/handoff-protocol.md` — процедура передачи.
- `meta/method-interaction-addendum.md` — процедура H3.
- `meta/changelog.md` — история.
- `meta/open-questions.md` — открытые вопросы.
- `PARTICIPANTS.md` — mapping псевдоним → модель.
- `corpus/` — публикационный слой.
- `METHOD.md` — протокол эксперимента.

## Что не сделано

- Группа B разбора Z:
  - Related work в corpus/en/ (краткий).
  - Заморозка METHOD (pending после replication).
- instruction-effect: закрыт 021 (anticipation NO).
- 022: уточняющий Named divergence (дизайн не начат).
- Публикация 021 в X: не сделана.
