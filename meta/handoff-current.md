# HANDOFF CURRENT

**Дата:** 2026-11-11
**Статус:** актуальный

Снимок текущего состояния LAB. Передаётся новому
ведущему при смене чата. Проверяется по §8
handoff-protocol.

## CURRENT STATE

    HEAD: 1f19fbc (main-working = origin/main)
    ACTIVE EXPERIMENT: none
    STATUS: closed
    LAST COMPLETED: 025 (закрыт, H6 не проверена
      через material-run)
    WORKING HYPOTHESES:
      - Named divergence: Luna A2=YES x4
        (020, 021, 023, 024). Replicated по §7.
        Sakana B=PARTIAL x3 + NO в 024. Паттерн
        ослаблен, не опровергнут.
      - No-default: supported 2/3, not universal.
        v2 — сходимость, причина не установлена.
        Гипотезы v2 (material-specific, frame-
        specific, active/passive, symmetry of
        stakes, positive vs negative duties) —
        не проверены. См. open-questions после 024.
      - 020 и 024 — L3 / preliminary. 021 и 023 —
        L2 / preliminary. 2:2. ND-L3 как класс
        не replicated.
      - Конкурентная: epistemic authority. Не
        проверена.
    KNOWN UNKNOWNs:
      - v2 — причина сходимости не установлена.
      - T-full NO/PARTIAL/YES — три режима,
        не нормативная сущность в §14.
      - Confound знания гипотезы: один случай.
    PENDING DECISION:
      - 026: смена ролей A/B на материале
        Named divergence. Единственный чистый
        тест «роль vs узел». Отложен с 020.
      - H6 — метка без проверки. Кандидат на
        другой метод (анализ текстов v1–v3
        из 023, не генерация новых).
      - Правило изоляции: любой прогон с LAB/
        hypothesis context → CONFOUND, не primary.
      - Заморозка METHOD — pending.
      - CURRENT STATE устаревает при каждом коммите;
        обновлять по мере значимых изменений.

## HEAD

- LAB: 1f19fbc (main-working = origin/main)
- blog: 6168e33 (main)

## Что сделано в сессии

Сессия: 2026-10-06 — 2026-11-11.

- L3 020 — принято решение: оставить без правок
  задним числом. §7 METHOD v4 разделяет уровень
  эксперимента (L3) и уровень устойчивости
  (preliminary). 021 ограничивает обобщение,
  но не отменяет классификацию 020.
- CORPUS POINT 020 — аннотация после 021 (ru+en
  одним коммитом): INTERACTION-ONLY как свойство
  класса не replicated. Ссылка на §14 addendum.
- Ветки сведены: одна линия main-working →
  origin/main. Ветка `main` на remote удалена
  (была ошибочно создана при первом пуше).
- 022 — семь preflight-итераций материала:
  - v1 (найм, X/Y): A=X, B=X. Стоп.
  - v2 (найм, X/Y выровнен): A=Y, B=Y. Стоп.
  - v3 (дедлайн): A=стабилизация, B=стабилизация.
  - v4 (утечка ПДн): отклонён внешними до preflight.
  - v5 (логистика): A=соблюсти, B=соблюсти.
  - v6 (спецификация vs экспертиза): A=не подписывать,
    B=не подписывать.
  - v7 (слот GPU, диспетчер без права):
    A=соблюсти, B=соблюсти.
  - v8 (бюджет регионов, руководитель с правом):
    A=перераспределить, B=перераспределить.
  - Батарея не запускалась. T-full / T-pre-R
    не измерялись.
- 022 закрыт как не давший third case Named
  divergence. Формулировка минимальная, без
  каузальных утверждений.
- Гипотеза no-default — рабочая, не проверенная.
  Объясняет все семь сходимостей и оба divergence
  (020/021), не прибегая к sacred или полномочиям.
- Зафиксировано:
  - `experiments/022-interaction/preflight-log.md`
    (журнал, данные, гипотезы).
  - `meta/open-questions.md` — раздел «Новые
    вопросы после 022 (preflight)».
- Уроки метода подбора материала:
  - Preflight при шести-семи сходимостях подряд
    переходит в подгонку. Лимит: до 3 preflight
    на материал, затем external review.
  - Sequential hypothesis search создаёт
    confirmation-by-material-design.
  - Blind design снимает priming, но не framing.
- Внешние (Luna, Grok, Kimi) отработали три
  раунда по 022: 1) пять развилок дизайна,
  2) полный черновик, 3) паттерн сходимостей
  и новая гипотеза. Все три рекомендовали
  зафиксировать паттерн и не продолжать подбор.
- 025 — проверка гипотезы H6 (locus of rule
  failure). Design-gate v1–v4: четыре документа,
  три раунда внешних, ноль прогонов. Отказ
  от design-gate, переход к пилотам.
  - Pilot 1 (L-after): сходимость, валиден.
    H6 prediction supported на одном локусе.
  - Pilot 2 (L-tie): сходимость, confounded.
    Содержательная асимметрия за формальным
    равенством.
  - Pilot 3 (L-tie): сходимость, confounded.
    Узел ввёл мета-правило (алфавит) вместо
    выбора из меню.
  - L-scope не проверялся. Граница размыта.
  - Контраст для H6 не получен.
- 025 закрыт через закрытие линии H6 в этой
  форме, не через снятие мортория. H6 —
  рабочая метка, не проверяемая гипотеза
  через material-run.
- Зафиксировано:
  - `experiments/025-interaction/pilot-log.md`
    (журнал, три пилота, финальный вывод).
  - `experiments/025-interaction/materials/`
    (pilot-1, pilot-2, pilot-3).
  - `meta/open-questions.md` — раздел «Новые
    вопросы после 025 (H6 не проверена)».
- Урок: процедура проверки не заменяет проверку.
  Design-gate v1–v4 — ноль прогонов. Пилоты —
  три прогона за то же время.

## Внешние системы

- X: @Shaen___. Пять постов: 019, 020, 021,
  023, 024. 022 не публиковался (third case
  не получен). Активность нулевая. Публикуется
  как фиксация, не для охвата.
- blog: https://shaenxxx-commits.github.io
  Posts: /019-trajectory/, /019-interaction/,
  /transcript-control/, /target-miss/,
  /020-named-divergence/, /021-named-divergence/,
  /022-named-divergence/, /023-no-default/,
  /024-no-default/ (коммит 6168e33).
- GitHub Pages: активен.
- CORPUS: публикационный слой в corpus/.
  ru/ + en/ + publications/.
  022 в CORPUS не отражён — third case не получен.

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
- `experiments/022-interaction/preflight-log.md` —
  журнал preflight 022.

## Что не сделано

Актуализировано 2026-11-11.

**Закрыто, не требует действий:**

- Related work в corpus/en/ — сделан
  (коммит a68bda1). Статус INTERPRETATION.
- POINT 022 в CORPUS — создан (коммит 8464289).
- Blog-пост 022 — сделан (/022-named-divergence/,
  коммит b4447d1).
- Проверка no-default — проведена в 023/024.
  Результат: replicated 2/3, не универсальна.
- H6 (locus of rule failure) — закрыта как
  непроверяемая через material-run (025).
- POINT 025 — не создаётся. 025 не дал
  результата для публикации: линия закрыта,
  не эксперимент с исходом. Запись в
  open-questions есть.

**METHOD — остаётся provisional freeze.**

Условие снятия (positive result 021 на новой
паре доменов) не выполнено. Named divergence
replicated как Target (Luna A2=YES ×4), но не
как L3-класс (2:2 по 020–024). Заморозка
невозможна по условию. Решение: оставить
provisional freeze, не пересматривать.
Записано здесь, чтобы не висело открытым.

**Открытое, требует решения о направлении:**

- Следующий эксперимент не определён.
  Кандидаты: 026 (смена ролей A/B), возврат
  к Named divergence с новым вопросом,
  стратегические вопросы (MAIA, CORPUS).
  Решение — за Оператором, не за ведущим.
- H6 — метка без проверки. Кандидат на другой
  метод (анализ текстов v1–v3 из 023,
  не генерация новых).
- Публикация в X: 022 и 025 не публиковались.
  Решение: не публиковать (нет результата
  для фиксации).
