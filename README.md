# Tuhfa — лендинг

Лендинг Telegram-сервиса виртуальных подарков в Узбекистане: подарочные сертификаты партнёров и анимационные подарки, оплата Click и Payme, языки RU / UZ.

Один статический файл `index.html` (HTML + CSS + JS), без сборки. Библиотеки подключаются с CDN: GSAP + ScrollTrigger (cdnjs), Lenis (unpkg), шрифты Google Fonts.

## Что заменить перед запуском

- Ссылки на бота — в начале скрипта в `index.html`:
  ```js
  var BOT_URL = 'https://t.me/';      // https://t.me/your_bot
  var PARTNER_URL = 'https://t.me/';  // https://t.me/your_bot?start=partner
  ```
- Узбекские тексты — объект `UZ` в скрипте (русские тексты лежат прямо в разметке).

## Деплой

Netlify публикует корень репозитория (`netlify.toml`, команда сборки не нужна). Каждый пуш в `main` обновляет сайт.
