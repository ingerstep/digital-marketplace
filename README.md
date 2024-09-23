# Digital marketplace

Digital marketplace — это веб-приложение как для покупателей, так и продавцов. Оно включает в себя полную функциональность для взаимодействия пользователей с продуктами и управления ими.

## Описание

Приложение состоит из нескольких экранов:

- **Авторизация**: Регистрация и аутентификация через почту как пользователь или продавец, c отправкой верификации через сервис Resend.
- **Основная страница**: Отображает продукты, корзину, регистрацию.
- **CMS**: Для управления продуктами, ролями пользователей через сервис Payload (доступна по роуту /sell).
- **Корзина**: Информация о добавленных товарах, редирект на оплату Stripe.
- **Страница спасибо**: После успешной оплаты, редирект на страницу спасибо.

## Установить репозиторий

```bash
$ git clone https://github.com/ingerstep/digital-marketplace
$ cd digital-marketplace
```

## Описание

Чтобы локально запустить проект, нужно подключить MongoDB и зарегистрироваться в сервисах Payload, Stripe, Resend.

```bash
# Необходимые ключи:
MONGODB_URL=
PAYLOAD_SECRET=
STRIPE_SECRET_KEY=
STRIPE_WEBHOOK_SECRET=
RESEND_API_KEY=
```

## Установка зависимостей

```bash
$ yarn install
```

## Запуск приложения

```bash
# development
$ yarn dev
```

## Cборка

```bash
$ yarn build
```

## Типы ts для Payload

```bash
$ yarn generate:types
```

## Зависимости

### Зависимости для работы
- **[@hookform/resolvers](https://www.npmjs.com/package/@hookform/resolvers)**: Ресолверы для интеграции с `react-hook-form`, обеспечивающие валидацию через схемы (например, Zod).
- **[@payloadcms/bundler-webpack](https://www.npmjs.com/package/@payloadcms/bundler-webpack)**: Вебпак-бандлер для проекта Payload CMS.
- **[@payloadcms/db-mongodb](https://www.npmjs.com/package/@payloadcms/db-mongodb)**: Адаптер для работы с базой данных MongoDB в Payload CMS.
- **[@payloadcms/richtext-slate](https://www.npmjs.com/package/@payloadcms/richtext-slate)**: Ричтекст-редактор, основанный на Slate.js, интегрированный в Payload CMS.
- **[@radix-ui/react-dialog](https://www.npmjs.com/package/@radix-ui/react-dialog)**: Компонент диалогового окна от Radix UI.
- **[@radix-ui/react-dropdown-menu](https://www.npmjs.com/package/@radix-ui/react-dropdown-menu)**: Компонент выпадающего меню от Radix UI.
- **[@radix-ui/react-label](https://www.npmjs.com/package/@radix-ui/react-label)**: Компонент метки для элементов формы от Radix UI.
- **[@radix-ui/react-scroll-area](https://www.npmjs.com/package/@radix-ui/react-scroll-area)**: Компонент прокручиваемой области от Radix UI.
- **[@radix-ui/react-separator](https://www.npmjs.com/package/@radix-ui/react-separator)**: Компонент-разделитель для создания визуального разделения содержимого от Radix UI.
- **[@radix-ui/react-slot](https://www.npmjs.com/package/@radix-ui/react-slot)**: Компонент для упрощения композиции сложных интерфейсов.
- **[@react-email/components](https://www.npmjs.com/package/@react-email/components)**: Компоненты для создания email-шаблонов в React.
- **[@tanstack/react-query](https://www.npmjs.com/package/@tanstack/react-query)**: Библиотека для управления состоянием сервера в React-приложениях.
- **[@trpc/client](https://www.npmjs.com/package/@trpc/client)**: Клиент для tRPC — библиотеки для построения типов интерфейсов в API.
- **[@trpc/next](https://www.npmjs.com/package/@trpc/next)**: Интеграция tRPC с фреймворком Next.js.
- **[@trpc/react-query](https://www.npmjs.com/package/@trpc/react-query)**: Интеграция tRPC с библиотекой `react-query` для управления состоянием API-запросов.
- **[@trpc/server](https://www.npmjs.com/package/@trpc/server)**: Серверная часть tRPC для построения API с использованием TypeScript.
- **[body-parser](https://www.npmjs.com/package/body-parser)**: Миддлвар для Express.js для парсинга тела запросов.
- **[class-variance-authority](https://www.npmjs.com/package/class-variance-authority)**: Утилита для управления CSS-классами с учетом различных вариаций.
- **[clsx](https://www.npmjs.com/package/clsx)**: Утилита для условного объединения CSS-классов.
- **[cross-env](https://www.npmjs.com/package/cross-env)**: Утилита для кроссплатформенной установки переменных окружения.
- **[date-fns](https://www.npmjs.com/package/date-fns)**: Библиотека для работы с датами в JavaScript.
- **[dotenv](https://www.npmjs.com/package/dotenv)**: Утилита для работы с переменными окружения из `.env` файлов.
- **[express](https://www.npmjs.com/package/express)**: Легкий веб-фреймворк для Node.js.
- **[lucide-react](https://www.npmjs.com/package/lucide-react)**: Набор иконок на основе SVG для React.
- **[next](https://www.npmjs.com/package/next)**: Фреймворк для серверного рендеринга и создания статических сайтов на React.
- **[nodemailer](https://www.npmjs.com/package/nodemailer)**: Библиотека для отправки электронных писем через Node.js.
- **[payload](https://www.npmjs.com/package/payload)**: CMS на базе Node.js и MongoDB для создания приложений с управлением контентом.
- **[react](https://www.npmjs.com/package/react)**: Библиотека для создания пользовательских интерфейсов.
- **[react-dom](https://www.npmjs.com/package/react-dom)**: Библиотека для взаимодействия React с DOM.
- **[react-hook-form](https://www.npmjs.com/package/react-hook-form)**: Библиотека для управления формами и валидацией в React.
- **[resend](https://www.npmjs.com/package/resend)**: Платформа для отправки писем через API с поддержкой React-шаблонов.
- **[sonner](https://www.npmjs.com/package/sonner)**: Библиотека для создания уведомлений в React-приложениях.
- **[stripe](https://www.npmjs.com/package/stripe)**: SDK для работы с платежами через Stripe API.
- **[swiper](https://www.npmjs.com/package/swiper)**: Библиотека для создания слайдеров и каруселей.
- **[tailwind-merge](https://www.npmjs.com/package/tailwind-merge)**: Утилита для объединения и приоритизации классов Tailwind CSS.
- **[tailwindcss-animate](https://www.npmjs.com/package/tailwindcss-animate)**: Плагин для добавления анимаций в Tailwind CSS.
- **[zod](https://www.npmjs.com/package/zod)**: Библиотека для валидации данных с использованием схем.
- **[zustand](https://www.npmjs.com/package/zustand)**: Легковесная библиотека для управления состоянием в React.

### Зависимости для разработки
- **[@types/express](https://www.npmjs.com/package/@types/express)**: Определения типов для Express.js.
- **[@types/node](https://www.npmjs.com/package/@types/node)**: Определения типов для Node.js.
- **[@types/nodemailer](https://www.npmjs.com/package/@types/nodemailer)**: Определения типов для Nodemailer.
- **[@types/react](https://www.npmjs.com/package/@types/react)**: Определения типов для React.
- **[@types/react-dom](https://www.npmjs.com/package/@types/react-dom)**: Определения типов для React DOM.
- **[copyfiles](https://www.npmjs.com/package/copyfiles)**: Утилита для копирования файлов.
- **[eslint](https://www.npmjs.com/package/eslint)**: Линтер для JavaScript и TypeScript.
- **[eslint-config-next](https://www.npmjs.com/package/eslint-config-next)**: Конфигурация ESLint для проектов на Next.js.
- **[nodemon](https://www.npmjs.com/package/nodemon)**: Утилита для автоматической перезагрузки серверов Node.js при изменении файлов.
- **[postcss](https://www.npmjs.com/package/postcss)**: Инструмент для трансформации CSS с использованием JavaScript-плагинов.
- **[tailwindcss](https://www.npmjs.com/package/tailwindcss)**: Фреймворк для создания адаптивных интерфейсов с использованием утилитарных классов.
- **[typescript](https://www.npmjs.com/package/typescript)**: Надстройка над JavaScript, добавляющая поддержку статических типов.
