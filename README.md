# Min's Collective

[![GitHub](https://img.shields.io/badge/GitHub-minkinad--collective-181717?logo=github&style=flat)](https://github.com/minkinad-collective)

Одностраничный сайт для организации, которая берёт на себя разработку сервисов и платформ под ключ.

## Локальный запуск

Сайт сделан как статический лендинг, поэтому его можно открыть напрямую через `index.html` или отдать любым простым HTTP-сервером.

Например:

```bash
cd we
python3 -m http.server 4173
```

После этого сайт будет доступен по адресу `http://localhost:4173`.

## CI и деплой

В репозитории настроены GitHub Actions:

- `CI` запускается на `push` в `main` и на `pull_request`, проверяет структуру `index.html` и синтаксис `main.js`.
- `Deploy to GitHub Pages` запускается на `push` в `main` и публикует статический сайт через GitHub Pages.

Для публикации убедитесь, что в настройках репозитория GitHub Pages использует режим `GitHub Actions`.
