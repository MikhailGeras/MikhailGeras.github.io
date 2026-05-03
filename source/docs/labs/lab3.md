# Лабораторная работа №3

## Цель работы

Реализовать автоматическое развертывание статического сайта, построенного на MkDocs, с использованием платформ SourceCraft и GitHub Actions.

## Выполненные действия

В ходе работы был создан и настроен статический сайт на MkDocs.

Исходные файлы сайта находятся в папке `source/docs`, конфигурационный файл MkDocs находится в `source/mkdocs.yml`.

В локальном Git-репозитории были настроены два удалённых репозитория:

- `origin` — репозиторий GitHub;
- `sourcecraft` — репозиторий SourceCraft.

Для GitHub был создан workflow `.github/workflows/deploy.yml`. При отправке изменений в ветку `main` GitHub Actions устанавливает зависимости, собирает сайт MkDocs и публикует его через GitHub Pages.

Для SourceCraft были созданы файлы `.sourcecraft/ci.yaml` и `.sourcecraft/sites.yaml`. SourceCraft CI при push в ветку `main` собирает сайт и публикует результат в ветку `release`. SourceCraft Sites берёт готовые HTML-файлы из папки `site` ветки `release`.

## Структура репозитория

```text
.
├── .github/
│   └── workflows/
│       └── deploy.yml
├── .sourcecraft/
│   ├── ci.yaml
│   └── sites.yaml
├── source/
│   ├── docs/
│   │   ├── index.md
│   │   └── lab3.md
│   └── mkdocs.yml
├── requirements.txt
└── README.md
```

## Ссылки

1. [Статический сайт на SourceCraft](https://mihaylogerasimov.sourcecraft.site/python2026-lr3/)
2. [Репозиторий на SourceCraft](https://sourcecraft.dev/mihaylogerasimov/python2026-lr3)
3. [Статический сайт на GitHub Pages](https://mikhailgeras.github.io/)
4. [Репозиторий на GitHub](https://github.com/MikhailGeras/MikhailGeras.github.io)