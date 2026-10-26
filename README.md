# 02-react-cafe

Віджет відгуків для Sip Happens Café, створений за допомогою Vite, React і TypeScript.

## Запуск

```bash
npm install
npm run dev
```

## Перевірки

```bash
npm run typecheck
npm run lint
npm run format:check
npm run build
```

`npm run preview` запускає локальний перегляд production-збірки після `npm run build`.

## Функціональність

- Кнопки Good, Neutral і Bad додають голос до відповідної категорії.
- Статистика показує кількість голосів, загальну суму й округлений відсоток позитивних відгуків.
- До першого голосу та після скидання показується «No feedback yet».
- Reset доступна тільки за наявності голосів і скидає всі три лічильники.
- Стан зберігається в App; дочірні компоненти отримують дані та колбеки через типізовані пропси.
- Після перезавантаження сторінки голосування починається з нуля.

Кожен компонент має окрему папку в `src/components` із файлами `.tsx` і `.module.css`. Спільні типи містяться в `src/types/votes.ts`.

CSS-модулі взято з [goitacademy/react-cafe-styles](https://github.com/goitacademy/react-cafe-styles); глобальну нормалізацію забезпечує `modern-normalize`.

## Публікація

Для здачі створіть репозиторій GitHub із назвою `02-react-cafe` та імпортуйте його у Vercel. Параметри: framework — Vite, build command — `npm run build`, output directory — `dist`.

Надайте посилання на репозиторій і розгорнутий застосунок. За умовами завдання після останнього `git push` зачекайте щонайменше 5 хвилин перед відправленням роботи на перевірку.
