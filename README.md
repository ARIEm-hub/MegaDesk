# MegaDesk Mobile v2

Исправленная версия сайта.

## Что исправлено

### 1. Мобильная верстка
Сайт принудительно включает мобильный интерфейс не только по ширине окна, но и по:
- touch input;
- pointer: coarse;
- navigator.maxTouchPoints;
- физическому размеру экрана;
- Android/iPhone user-agent.

Это помогает даже если в браузере случайно включена «Версия для ПК».

### 2. Кнопка запуска Bitrix24

Android:
`intent://#Intent;scheme=bitrix24;package=com.bitrix24.android;end`

Используется официальный Android package Bitrix24:
`com.bitrix24.android`

Browser fallback намеренно отсутствует.

iPhone:
`bitrix24://`

### 3. Инструкция

После открытия Bitrix24:
Меню -> Маркет -> MegaDesk -> Создать заявку

## GitHub Pages

Замените старый `index.html` этим файлом, сделайте Commit в `main`,
дождитесь завершения Pages deployment и откройте сайт заново.
