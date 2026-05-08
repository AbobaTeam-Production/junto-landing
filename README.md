# junto-landing

Лендинг проекта Junto — статический HTML.

## Стек

Чистый HTML/CSS, без сборки. Один файл `index.html` + две placeholder-страницы (`privacy.html`, `terms.html`). Шрифты с CDN (Google Fonts + Fontshare).

## Деплой

GitHub Pages из ветки `main` (workflow `.github/workflows/pages.yml`). При push в `main` Pages автоматически перевыкладывается.

Кастомный домен — через файл `CNAME` в корне (например, `juntoapp.tech`). Если хочется хостить с VPS вместо Pages — копируй `index.html` в `/srv/junto/landing/` и nginx раздаёт статику.

## Ссылки на скачивание

Лендинг ссылается на GitHub Releases репозитория `AbobaTeam-Production/junto-frontend`:

```
https://github.com/AbobaTeam-Production/junto-frontend/releases/latest/download/junto-android.apk
https://github.com/AbobaTeam-Production/junto-frontend/releases/latest/download/junto-windows-setup.exe
https://github.com/AbobaTeam-Production/junto-frontend/releases/latest/download/junto-linux.AppImage
```

`/releases/latest/download/<name>` всегда указывает на свежий релиз — лендинг править не нужно при выходе новой версии.
