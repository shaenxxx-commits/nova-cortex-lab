# HANDOFF CURRENT

**Дата:** 2026-10-08
**Статус:** актуальный

Снимок текущего состояния LAB. Передаётся новому
ведущему при смене чата. Проверяется по §8
handoff-protocol.

## CURRENT STATE

    HEAD: 135f84b (main-working = origin/main)
    ACTIVE EXPERIMENT: none
    STATUS: closed
    LAST COMPLETED: related-work POINT
      (corpus/ru + en, коммит a68bda1)
    WORKING HYPOTHESES:
      - Named divergence: роль A2 (Luna) YES x2,
        роль B (Sakana) PARTIAL x2. Preliminary, n=2.
      - No-default: divergence требует ситуации, где
        формальное правило молчит или исчерпано.
        Рабочая, не проверенная. См. preflight-log 022.
      - 020 — L3 / preliminary, INTERACTION-ONLY
        в рамках эксперимента. Не replicated как
        свойство класса.
    KNOWN UNKNOWNs:
      - Гипотеза no-default не проверена на новом
        материале.
      - v7 confounded: формулировка роли сама
        подсказывала ответ.
    PENDING DECISION:
      - Заморозка METHOD — pending после replication.
      - Проверка гипотезы no-default — отдельная
        серия (023), требует чистого дизайна.
      - CURRENT STATE устаревает при каждом коммите;
        обновлять по мере значимых изменений.
    LAST RESPONSE NUMBER: 190 в этом чате.

## HEAD

- LAB: 135f84b (main-working = origin/main)
- blog: b4447d1 (main)

## Что сделано в сессии

Сессия: 2026-10-06 — 2026-10-08.

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

## Внешние системы

- X: @Shaen___. Три поста: 019, 020, 021.
  Активность нулевая. Публикуется как фиксация,
  не для охвата. 022 не публиковался.
- blog: https://shaenxxx-commits.github.io
  Posts: /019-trajectory/, /019-interaction/,
  /transcript-control/, /target-miss/,
  /020-named-divergence/, /021-named-divergence/,
  /022-named-divergence/ (коммит b4447d1).
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

- Группа B разбора Z:
  - Related work в corpus/en/ — сделан
    (`corpus/ru/related-work.md` + `corpus/en/related-work.md`,
    коммит a68bda1). Статус INTERPRETATION.
  - Заморозка METHOD (pending после replication).
- Проверка гипотезы no-default — отдельная серия,
  не 022. Требует материала, где правило молчит
  или исчерпано, без sacred и без escape.
- POINT 022 в CORPUS — создан (ru + en + README,
  коммит 8464289). Статус OPEN. Формат:
  «preflight series, third case not obtained,
  no-default hypothesis». Ссылка на preflight-log.
- Blog-пост по POINT 022 — сделан
  (/022-named-divergence/, коммит b4447d1).
- Публикация 022 в X — не планируется. 021
  в X опубликован (три поста: 019, 020, 021).
