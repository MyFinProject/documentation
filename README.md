
# 💰 MyFinProject

> "Финансы поют романсы? - тогда тебе поможет наш проект!"


MyFinProject  — это фронт-часть приложения для управления личными финансами.


# 📘 Документация проекта MyFinProject

> Этот репозиторий содержит **проектную документацию** для веб-приложения MyFinProject — сервиса управления личными финансами. Здесь фиксируются бизнес-требования, архитектура, а также прогресс по Roadmap.

---

## 📁 Структура документации

```bash
docs/
├── README.md                  # Введение + инструкция
├── roadmap.md                 # Роадмап
├── work_shedule.md            # График работ в соответствии с чекпоинтами
├── business_requirements.md   # Бизнес-требования
├── architecture.md            # Архитектура и технологии
├── ERD DataBase.md            # ERD БД
└── figma-link.md              # Ссылка на макет
```
---

## 📝 Инструкция к проекту MyFinProject

> Этот раздел поможет вам **запустить, протестировать и понять**, как устроен проект с технической стороны. Независимо от того, backend вы или frontend, вы не потеряетесь.



### 📦 Репозитории проекта

| Часть         | Ссылка                                                          | Назначение                          |
|---------------|------------------------------------------------------------------|-------------------------------------|
| 📘 Документация | [github.com/MyFinProject/documentation](https://github.com/MyFinProject/documentation)         | Бизнес-логика, архитектура, ERD     |
| 💡 Backend     | [github.com/MyFinProject/backend](https://github.com/MyFinProject/backend)     | ASP web Api               |
| 🎨 Frontend    | [github.com/MyFinProject/frontend](https://github.com/MyFinProject/frontend)   | Vue 3, Pinia, Axios, Tailwind CSS   |

## Фичи
1) скан чеков
2) приятный дизайн
3) авторизация с проверкой почты
4) цели
5) добавление кастомных категорий

## 🖥️ Как запустить проект локально

### ⬇️ 1. Клонируйте оба репозитория

```bash
git clone https://github.com/MyFinProject/backend.git
git clone https://github.com/MyFinProject/frontend.git
```

2. **Настроить строку подключения**

Откройте appsettings.Development.json и пропишите:
> "ConnectionStrings": {
"DefaultConnection": "Server=localhost;Database=MyFinDb;User Id=sa;Password=YourStrong@Passw0rd;"
}

3. **Применить миграции и инициализировать базу**
>dotnet ef database update


4. **Запуск приложения**
>dotnet run --project Api
