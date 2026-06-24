---
title: PM 4 — Agile-методологии
---

# PM 4 — Agile-методологии

Источник: `raw/Lectures Summaries/pm_4 Agile Methodologies.md`, `raw/Slides/PM 4 Agile methodologies.pptx.pdf`, `raw/Slides/Agile Frameworks_PM Tasks.pdf`, `raw/Transcriptions/Копия PM 4 Agile methodologies.txt`.

Четвёртое занятие курса [[pm-it-course]]. Тема — семейство Agile-фреймворков: повтор различий [[waterfall]] vs [[agile]], затем подробный разбор Scrum, Kanban, Scrumban, XP, Lean и масштабируемых фреймворков (LeSS, SAFe, Nexus). Выбор конкретного фреймворка зависит от размера команды, типа проекта, зрелости Agile-практик и типа контракта ([[contract-types]]).

## Ключевые темы
- **Waterfall vs Agile** — повтор материала [[pm-3-methodologies]]: каскад vs итерации.
- **Scrum** — >65% команд по Annual State of Agile Report; происхождение термина из регби; Scrum Guide (Сазерленд, Швабер); 8 шагов внедрения Scrum по Сазерленду; роли, артефакты, 5 событий (на этой лекции спринт ещё описан как 1–2 недели и события — числом 5 с Backlog Refinement отдельно не выделен); условия эффективного применения. Подробно см. [[scrum]] (страница объединяет эту лекцию и [[pm-5-scrum]], где материал расширен и уточнён).
- **Kanban** — происхождение с заводов Toyota (1950-е), 4 принципа (точно в срок, наглядность, равномерная нагрузка, постоянное улучшение), WIP-лимиты и управление узкими местами, инструменты (Trello, Jira, Asana). См. [[kanban]].
- **Scrumban** — гибрид Scrum (структура, роли, спринты) и Kanban (доска, WIP-лимиты). См. [[scrumban]].
- **XP (Extreme Programming)** — только для разработки ПО; TDD, парное программирование, continuous integration, рефакторинг, частые малые релизы, коллективное владение кодом, единые стандарты кода; заказчик — конечный пользователь, постоянно на связи. Сравнение с Scrum/Kanban/Lean. См. [[xp]].
- **Lean** — философия (не методология) бережливого мышления; 6 видов потерь, адаптированных к IT (в исходных слайдах — классические 8 видов потерь производства + отдельно адаптация к IT в 6 категорий, см. [[lean]] о расхождении в количестве).
- **Масштабирование Agile** — LeSS, SAFe (Team/Program/Portfolio, PI Planning, Confidence Vote), Nexus (Nexus Integration Team, Nexus Daily Scrum, Nexus Sprint Backlog), а также кратко упомянуты Scrum of Scrums и Disciplined Agile Delivery. См. [[scaling-frameworks]].

## Практические задания (очное занятие)
7 заданий: выбор методологии для продуктового стартапа; Sprint Planning и Sprint Backlog для B2B SaaS; настройка Kanban-доски и WIP-лимитов для команды поддержки; Lean-аудит процесса разработки; внедрение XP-практик в команду с техдолгом; переход со Scrum на Scrumban; выбор масштабируемого фреймворка (LeSS/SAFe/Nexus) для финтех-проекта.

Файл `raw/Slides/Agile Frameworks_PM Tasks.pdf` содержит те же 7 заданий в распечатываемом формате — отдельной source-страницы для него не создавалось (дублирует summary, как и в случае с PM 2/PM 3).

## Связанные страницы
- [[pm-it-course]]
- [[pm-3-methodologies]]
- [[pm-5-scrum]]
- [[scrum]], [[kanban]], [[scrumban]], [[xp]], [[lean]], [[scaling-frameworks]]
- [[agile]], [[waterfall]], [[contract-types]]
