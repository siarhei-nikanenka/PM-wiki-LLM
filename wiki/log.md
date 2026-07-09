# Log

Апенд-онли журнал операций над вики. Формат каждой записи:

```
## YYYY-MM-DD operation | title
краткое описание изменения / какие страницы созданы/обновлены
```

Где `operation` — одно из: `ingest`, `query`, `lint`, `revise`.

---

## 2026-06-17 ingest | PM 1 Intro, PM 2 Main Notions, PM 3 Methodologies
Поглощены все материалы из raw/ по курсу «Управление проектами в IT» (3 лекции: summary + slides + транскрипты/tasks-pdf для каждой).
Создано:
- sources: pm-1-intro.md, pm-2-main-notions.md, pm-3-methodologies.md
- entities: sergey-nikonenko.md, pm-it-course.md, pmbok.md
- concepts: it-company-types.md, project-vs-process.md, iron-triangle.md, scope-creep.md, project-estimation.md, stakeholders.md, pm-role.md, waterfall.md, agile.md, agile-manifesto.md, velocity-metrics.md, contract-types.md
Обновлены: index.md, overview.md.
Примечание: raw/Slides/pm_tasks.pdf и Methodologies_PM Tasks.pdf дублируют практические задания, уже перечисленные в summary-файлах лекций 2 и 3 — отдельных source-страниц для них не создавалось, они отражены как часть pm-2-main-notions.md и pm-3-methodologies.md.

## 2026-06-18 query | слайды по типам контрактов
Пользователь спросил, какие слайды раскрывают тему Fixed Price vs T&M. При проверке raw/Slides/PM 3 Methodologies.pdf (слайды 27-31) нашлась более подробная информация, чем была законспектирована: таблицы параметров (неизменяемые/изменяемые, гибкость, риски) для каждого типа контракта и четвёртый тип — FFF (Fixed time, Fix budget, Flex-scope), которого не было в текстовом резюме лекции.
Обновлено: concepts/contract-types.md (добавлены параметры и тип FFF), index.md (описание страницы).

## 2026-06-18 query | знакомство со студентами на PM 1 Intro
Пользователь спросил, как зовут студентов и что каждый о себе рассказывал. В транскрипте `raw/Transcriptions/youtube_yt_4d887e59.txt` (~строки 217-281) нашлись самопрезентации 6 студентов. После уточнений пользователя исправлены ошибки распознавания: первый студент — Дмитрий (не Римон), 8 лет в общепите (факт про триатлон относился к преподавателю, а не к студенту); Наталья — политолог-юрист (не «паритолог-юрист»).
Обновлено: sources/pm-1-intro.md (добавлен раздел «Знакомство со студентами группы»), index.md (описание страницы).

## 2026-06-24 ingest | PM 4 Agile Methodologies, PM 5 Scrum
Поглощены материалы лекций 4 и 5 курса «Управление проектами в IT» (summary + slides + транскрипты + tasks-pdf для каждой).
Создано:
- sources: pm-4-agile-methodologies.md, pm-5-scrum.md
- concepts: scrum.md, kanban.md, scrumban.md, xp.md, lean.md, scaling-frameworks.md
Обновлены: concepts/agile.md (ссылки на новые страницы конкретных фреймворков), overview.md (абзац про Agile-фреймворки), index.md.
Примечания:
- raw/Slides/Agile Frameworks_PM Tasks.pdf и Scrum Framework_PM Tasks.pdf дублируют практические задания, уже перечисленные в summary лекций 4 и 5 — отдельных source-страниц для них не создавалось (та же логика, что и для pm_tasks.pdf / Methodologies_PM Tasks.pdf в предыдущем ingest).
- PM 5 уточняет и местами не совпадает с PM 4: PM 4 называет роль «Development Team» и говорит про 5 событий Scrum (включая сам спринт, спринт 1–2 недели); PM 5 (более новая и подробная) использует термин «Developers» (актуальный Scrum Guide), выделяет 4 формальных события внутри контейнера «Спринт» (≤1 месяц, золотой стандарт 2 недели) и отдельно описывает Backlog Refinement. В concepts/scrum.md за основу взята версия PM 5, расхождение отражено в sources/pm-5-scrum.md.
- В слайдах PM 4 (`PM 4 Agile methodologies.pptx.pdf`) для Lean даны классические 8 видов потерь производства, а в тексте лекции и в адаптации к IT на тех же слайдах — 6 видов; расхождение зафиксировано в concepts/lean.md.

## 2026-06-25 lint
Проверка вики после ingest PM 6 SDLC.
Находки:
- Сирот не найдено — все страницы присутствуют в index.md и имеют входящие ссылки.
- Противоречий не найдено (два ранее известных расхождения PM4/PM5 и 6/8 потерь Lean остаются задокументированными).
- Устаревших данных не найдено.
- Недостающие кросс-ссылки — исправлены:
  - entities/pm-it-course.md (тема 4 программы → добавлены ссылки на [[sdlc]] и [[pm-6-sdlc]])
  - concepts/xp.md (Continuous Integration как практика XP → добавлена связь с [[cicd]])
  - concepts/version-control.md (PR/Code Review → добавлена связь с [[xp]] как источником практики CI и коллективного владения кодом)
- Обновлено: index.md (описание waterfall уточнено с учётом SDLC-контекста).

## 2026-06-25 ingest | PM 6 SDLC
Поглощены материалы лекции 6 курса «Управление проектами в IT» (summary + slides + транскрипт).
Создано:
- sources: pm-6-sdlc.md
- concepts: sdlc.md, devops.md, cicd.md, version-control.md
Обновлены: concepts/waterfall.md (добавлен блок «Водопад в контексте SDLC», риски и способы снижения), index.md, overview.md (новый абзац «Техническая основа: SDLC и инструменты команды»).

## 2026-06-24 lint
Проверка вики после ingest PM 4/PM 5: противоречия, устаревшие данные, страницы-сироты, недостающие кросс-ссылки.
Находки:
- Сирот не найдено — все страницы concepts/entities/sources присутствуют в index.md и имеют входящие ссылки.
- Новых противоречий не найдено; два известных расхождения (PM4 vs PM5 по числу событий Scrum/названию роли developers; 6 vs 8 видов потерь Lean) уже зафиксированы в ingest-записи выше и являются естественной эволюцией материала лектора, а не ошибкой.
- Устаревших данных не найдено.
- Недостающие кросс-ссылки — исправлены: concepts/contract-types.md (T&M → ссылка на scrum.md), concepts/it-company-types.md (роль Scrum Master → ссылка на scrum.md, добавлен блок «Связанные страницы»), concepts/velocity-metrics.md (velocity как вход Sprint Planning → ссылка на scrum.md), entities/pm-it-course.md (уточнено, что тема 3 программы курса фактически растянулась на три занятия — pm-3/4/5).

## 2026-07-09 ingest | PM 7 Discovery/Initiation, PM 8 Stakeholders, PM 9 Project Integration
Поглощены материалы лекций 7, 8 и 9 курса «Управление проектами в IT» (summary + slides + транскрипты для каждой).
Создано:
- sources: pm-7-discovery-and-initiation.md, pm-8-stakeholders.md, pm-9-project-integration.md
- concepts: rfx.md, discovery-phase.md, wbs.md, project-charter.md, kickoff-meeting.md, stakeholder-matrices.md, raci-daci.md, team-charter.md, pmbok-process-groups.md, knowledge-management.md, project-closure.md
Обновлены:
- concepts/stakeholders.md — существенно расширена (была основана только на pm-2-main-notions): добавлена теория Фримана, 4 процесса PMBOK 6, подход PMBOK 7, итеративный цикл вовлечения, реестр стейкхолдеров, 5 уровней вовлечённости, типичные ошибки, soft skills.
- entities/pmbok.md — добавлены пять стадий/процессных групп PMBOK 6 и Performance Domains PMBOK 7.
- entities/pm-it-course.md — добавлены ссылки на pm-7/8/9; зафиксировано расхождение нумерации: тема 8 программы («Распределение ролей») по факту целиком посвящена стейкхолдерам, а тема 9 («Soft Skills») по факту — управлению интеграцией и процессным группам PMBOK (продолжение расхождения, впервые отмеченного для тем 3–5).
- concepts/project-vs-process.md, concepts/pm-role.md — добавлены ссылки на pm-9-project-integration (pm-role.md: метафора «дирижёра оркестра» формализована как управление интеграцией).
- overview.md — добавлены три абзаца: «Инициация проекта: от первого контакта до kickoff», «Стейкхолдеры: от идентификации до soft skills», «Интеграция и завершение проекта».
- index.md — добавлены все новые страницы.
Примечания:
- raw/Slides/PM 7–9 *.pptx.pdf не создавали отдельных source-страниц (та же логика, что и для предыдущих слайдов — они дублируют содержание Lectures Summaries и упомянуты как источник в соответствующих sources/pm-N-*.md).
- Обнаружено и исправлено попутно: `raw/Transcriptions/Копия PM 6 SDLC.txt.done` был переименован пользователем в `.txt` (содержимое идентично); ссылки на этот файл в sources/pm-6-sdlc.md и index.md обновлены на новое имя.
- Реестр стейкхолдеров (PM8) и уровни вовлечённости не противоречат карте стейкхолдеров из pm-2-main-notions — второй является более простой, ранней версией того же инструмента; concepts/stakeholders.md сохраняет обе ссылки на источники.

## 2026-07-09 lint
Проверка вики после ingest PM 7/8/9: противоречия, устаревшие данные, страницы-сироты, недостающие кросс-ссылки (полная проверка всех [[ссылок]] в wiki/ скриптом, не только новых страниц).
Находки:
- Битых `[[ссылок]]` не найдено (все цели существуют как файлы).
- Сирот не найдено — каждая страница concepts/entities/sources имеет хотя бы одну входящую ссылку помимо index.md.
- Противоречий не найдено. Точки потенциального расхождения проверены отдельно и признаны непротиворечивыми: (а) реестр стейкхолдеров PM8 vs карта стейкхолдеров PM2 — второй является более ранним и простым вариантом того же инструмента, конфликта нет; (б) «пять стадий PMBOK 6» (PM7, неформально) vs «пять процессных групп» (PM9, формально, подчёркнуто «не фазы, могут пересекаться») — не противоречие, а уточнение терминологии, отражено в entities/pmbok.md.
- Устаревших данных не найдено.
- Недостающие кросс-ссылки — исправлены:
  - concepts/scope-creep.md — добавлены ссылки на [[discovery-phase]] (Product Vision), [[rfx]] (assumptions), [[project-closure]] (scope creep после сдачи проекта).
  - concepts/contract-types.md — в разделе Fixed Price добавлена ссылка на [[discovery-phase]].
  - concepts/project-estimation.md — добавлен абзац про PERT-оценку задач со ссылкой на [[rfx]].
  - concepts/scrum.md — добавлен раздел «Scrum и PMBOK» со ссылками на [[pmbok-process-groups]] и [[knowledge-management]] (события Scrum как зеркало процессных групп PMBOK и как инструмент управления знаниями).
  - concepts/waterfall.md — упоминание WBS превращено в ссылку на [[wbs]], добавлено в «Связанные страницы».
