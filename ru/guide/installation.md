---
title: Установка
description: Nuxt.js действительно легко начать использовать. Просто проект требует только подключения зависимости `nuxt`.
---

> Nuxt.js действительно легко начать использовать. Просто проект требует только подключения зависимости `nuxt`.

## Использование стартового шаблона приложения Nuxt.js

Для быстрого начала, команда Nuxt.js создала [стартовый шаблон приложения](https://github.com/nuxt-community/starter-template).

[Скачайте .zip](https://github.com/nuxt-community/starter-template/archive/master.zip) стартового шаблона или установите его с помощью vue-cli:

```bash
$ vue init nuxt-community/starter-template <project-name>
```

> Если [vue-cli](https://github.com/vuejs/vue-cli) не установлена, то установите её сначала командой `npm install -g vue-cli`

затем установите зависимости:

```bash
$ cd <project-name>
$ npm install
```

и запустите проект:
```bash
$ npm run dev
```

Приложение будет запущено по адресу http://localhost:3000

<p class="Alert">Nuxt.js будет отслеживать изменения файлов внутри каталога `pages`, поэтому нет необходимости перезпускать приложение при добавлении новых страниц.</p>

Чтобы узнать больше о структуре каталогов проекта: [Документация по структуре каталогов](/guide/directory-structure).

## Создание с нуля

Создать Nuxt.js приложение с нуля также достаточно просто, это требует *1 файла и 1 каталога*. Давайте создадим пустой каталог для начала работы над приложением:

```bash
$ mkdir <project-name>
$ cd <project-name>
```

*Примечание: замените project-name на название вашего проекта.*

### Файл package.json

Проект требует созданного файла `package.json` для определения как запускать `nuxt`:
```json
{
  "name": "my-app",
  "scripts": {
    "dev": "nuxt"
  }
}
```
`scripts` будет запускать Nuxt.js с помощью команды `npm run dev`.

### Установка `nuxt`

После того как файл `package.json` будет создан, добавьте в проект `nuxt` через npm:
```bash
npm install --save nuxt
```

### Каталог `pages`

Nuxt.js будет преобразовывать каждый `*.vue` файл внутри каталога `pages` в маршрут для приложения.

Создайте каталог `pages`:
```bash
$ mkdir pages
```

затем создайте первую страницу в `pages/index.vue`:
```html
<template>
  <h1>Hello world!</h1>
</template>
```

и запустите проект командой:
```bash
$ npm run dev
```
Приложение будет запущено по адресу http://localhost:3000

<p class="Alert">Nuxt.js будет отслеживать изменения файлов внутри каталога `pages`, поэтому нет необходимости перезпускать приложение при добавлении новых страниц.</p>

Чтобы узнать больше о структуре каталогов проекта: [Документация по структуре каталогов](/guide/directory-structure).
