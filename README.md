# PhotoAI — Лендинг сайт

Статический лендинг для PhotoAI. Деплоится автоматически на GitHub Pages при пуше в `main`.

## Деплой

1. Создайте репозиторий `photoai-ru/photoai-landing` на GitHub
2. Загрузите файлы: `git push origin main`
3. В настройках репо: **Settings → Pages → Source → GitHub Actions**
4. Через ~1 минуту сайт будет доступен на `https://photoai-ru.github.io/photoai-landing`

## Настройка домена (если есть)

Добавьте файл `CNAME` с содержимым `photoai.ru` и настройте DNS:
```
A     @   185.199.108.153
A     @   185.199.109.153
CNAME www photoai-ru.github.io
```

## Структура

```
index.html      — одностраничный лендинг (всё inline)
.github/
  workflows/
    deploy.yml  — автодеплой на GitHub Pages
README.md
```
