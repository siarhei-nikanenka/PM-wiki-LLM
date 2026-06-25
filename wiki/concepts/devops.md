---
title: DevOps
---

# DevOps

Из [[pm-6-sdlc]].

**DevOps** — культура (и набор практик) на стыке разработки (Dev = Developers & Testers) и эксплуатации (Ops = IT Operations). Цель — устранить барьер между командами и ускорить безопасную доставку кода в production.

---

## 8-этапный бесконечный цикл DevOps

```
Plan → Code → Build → Test → Release → Deploy → Operate → Monitor → (Plan...)
```

| Этап | Инструменты |
|------|------------|
| Plan | Jira, Trello |
| Code | Git, GitHub, VS Code, IntelliJ |
| Build | Jenkins, Maven |
| Test | Selenium, JUnit |
| Release | Jenkins, GitLab, GitHub Actions |
| Deploy | Docker, Kubernetes, Jenkins, Azure DevOps |
| Operate | Docker, Kubernetes |
| Monitor | Grafana, Prometheus, Google Analytics |

---

## Build vs Release

- **Build** — собранное приложение, переданное командой разработки команде тестирования. Один релизный цикл может включать несколько build.
- **Release** — официальный выпуск для конечных пользователей. Build становится Release только после тестирования и сертификации командой QA.

> Пример: за два дня создали 5 build. Build №3 — критичный баг в оплате, №4 — мелкие баги, №5 прошёл все тесты. Release = build №5.

---

## Deployment Management vs Release Management

**Deployment Management** — техническая операция:
> Moving, installing and configuring of new/changed software, hardware and documentation or any other service component to target environment.

**Release Management** — весь процесс обеспечения готовности сервиса для публичного использования. 8-этапный цикл:

```
1. Request for Changes / New Features
2. Release Planning & Design
3. Software Build
4. Review
5. Test
6. Deployment
7. Support
8. Issue Reporting & Collection
```

Deployment Management — это лишь шаг 6 внутри Release Management.

---

## Software Environments

**Software Environment** — совокупность аппаратных и программных инструментов, используемых разработчиком для создания систем.

| Среда | Назначение |
|-------|-----------|
| **Development** | Эксперименты разработчиков, нестабильный код |
| **Staging / PreProd** | Максимально близка к production; здесь проходит финальная проверка и UAT |
| **Production** | Рабочая среда для конечных пользователей |

Изоляция сред снижает риск попадания нестабильного кода к пользователям.

---

## Связанные страницы
- [[sdlc]] — этапы SDLC, связь с DevOps
- [[cicd]] — CI/CD как часть DevOps (этапы Build/Test/Release/Deploy)
- [[version-control]] — Code-этап DevOps
- [[pm-6-sdlc]]
