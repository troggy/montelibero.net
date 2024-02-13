# Source code for montelibero.me

## Development

```sh
npm install
npm start
```

## Structure

`_data/metatada.json`            — common metadata for the website. List of languages is here

`_data/navigation.json`          — top navigation for all the locales

`_includes/layouts/base.njk`     — base layout (common parts for all the layouts)

`_includes/layouts/home.njk`     — specific layout for home page

`_includes/layout/secondary.njk` — specific layout for all the secondary pages

`content/en/`                    — content in English. Each *.md file renders as a page

`content/en/en.toml`             - localized strings for English locale. Includes the page blocks for home page in English

`content/ru/`                    — content in Russian. Each *.md file renders as a page

`content/ru/ru.toml`             - localized strings for Russian locale. Includes the page blocks for home page in Russian

`netlify.toml`                   - config for [Netlify deployment](https://docs.netlify.com/configure-builds/file-based-configuration/). Contains build settings and rules for language-specific redirects

`eleventy.config.js`              - [Eleventy config](https://www.11ty.dev/docs/config/)

## Editing content

Редакторы работают c текстами только в файлами в папке `content`, а также дополнительно могут положить медиа-файлы в папку `public/`. 

Базовый сценарий таков:

Редактор вносит правки в контент на русском языке в папке `/content/ru/`. Например, используя встроенный редактор гитхаба: https://github.com/troggy/montelibero.me/edit/master/content/ru/ru.toml (пример для стартовой страницы). 

Для сохранения правок создаётся гит-ветка
![Screen Recording 2024-02-12 at 23 55 29](https://github.com/troggy/montelibero.me/assets/163447/e20e3f46-a909-4649-8a2c-3098ed7fe42d)


## Production deployment

