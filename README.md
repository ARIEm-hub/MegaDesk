# MegaDesk GitHub Pages launcher

Статическая страница для QR-кода и перехода к MegaDesk.

## Что делает

- Android: по нажатию кнопки пытается передать URL MegaDesk напрямую приложению Bitrix24
  через Android Intent с package `com.bitrix24.android`.
- iPhone/iPad: открывает Bitrix24 через `bitrix24://`.
- Desktop: открывает веб-адрес MegaDesk.

## Ограничение Bitrix24

У мобильного Bitrix24 нет публичного внешнего deep-link, который гарантированно открывает
произвольную внутреннюю страницу/Marketplace-приложение из внешнего сайта.

Поэтому:

- Android — прямой переход в MegaDesk может заработать только если установленная версия
  Bitrix24 принимает URL портала через соответствующий intent.
- iOS — `bitrix24://` открывает приложение, но не гарантирует автоматический переход
  прямо в MegaDesk.

Сайт специально НЕ использует автоматический browser fallback на мобильных устройствах,
чтобы кнопка «Открыть MegaDesk» не отправляла пользователя в веб-версию при неудаче.

## Публикация на GitHub Pages

1. Создайте новый репозиторий, например `megadesk`.
2. Загрузите `index.html` в корень репозитория.
3. Откройте:
   Settings -> Pages
4. В Source выберите:
   Deploy from a branch
5. Branch:
   `main`
6. Folder:
   `/(root)`
7. Сохраните.

Ссылка будет примерно:

`https://USERNAME.github.io/megadesk/`

Эту ссылку можно зашить в QR-код.

## MegaDesk

Портал:
`https://portal.dasm.kz`

Страница:
`https://portal.dasm.kz/marketplace/app/82/`
