# Шаблоны для лекций AHJ

Набор шаблонов для проведения лекций по AHJ

## Содержание

* [x] [Рабочее окружение](/workspace)
* [x] [DOM](/dom)
* [x] [Events](/events)
* [x] [Testing](/testing)
* [x] [Forms](/forms)
* [x] [DnD](/dnd)
* [x] [HTTP](/http)
* [x] [Animations](/anim)
* [x] [Geolocation, Notification, Media](/geo)
* [x] [RxJS](/rxjs)
* [x] [SSE, WS](/sse-ws)
* [ ] [Web Workers, Service Workers](/workers)

По всем вопросам обращайтесь к @coursar.

## Как использовать

1. Склонируйте репозиторий
1. Перейдите в каталог интересующей вас лекции
1. Запустите `npm install` для установки зависимостей
1. Запустите `npm start` для старта frontend'а в режиме разработки, `npm run watch` для старта backend'а в режиме разработки
1. Запустите `npm build` для сборки (только для frontend'а)
1. Запустите `npm test` для прогона тестов (только для frontend'а)

*Важно*: в некоторых лекциях (HTTP, SSE + WS), предполагается наличие серверной части. Для таких лекций внутри каталога идёт деление на frontend/backend. Это значит, что `npm install` нужно делать и для frontend'а и для backend'а.


## Что такое шаблоны и для чего?

Все лекции продвинутого уровня построены на обучении реальным навыкам, а не работе в песочнице. Поэтому все студенты с первых лекций используют инфраструктуру, максимально похожую на промышленную:
* npm/yarn
* git
* babel, core-js и полифиллы
* eslint
* jest
* jsdom
* puppeeter
* webpack
* webpack-dev-server
* continuous integration/deployment

Поэтому для всех лекций, кроме тех, где это отдельно оговорено (например, DOM), лекторам необходимо использовать заранее подготовленный шаблон, чтобы не возиться с настройкой вручную и не показывать код в "консольке браузера".

Мы делаем практический курс, который не оторван от жизни. Курс про то, как разработка строится в реальной жизни с:
* редактором кода (или IDE)
* npm
* git/GitHub
* Code Style
* Code Review
* CI/CD

Обязательно:
* при демонстрации на лекциях использовать базовый шаблон
* в качестве среды разработки использовать VSCode со светлой темой оформления и подключенным плагином ESLint

Недопустимо:
* использовать сервисы jsbin.com, repl.it и аналогичные для демонстрации
* отключение linter'а
* демонстрация через открытие файла html в браузере (file://)

Зачем: мы стремимся сделать курс для студентов, чтобы студент смог понять и повторить то, что вы делаете на лекции, не тратя кучу времени на то, чтобы разобраться:
* как настроен ваш проект
* как настроен ваш редактор кода
* и почему с него требуют ESLint и CodeStyle в домашках, а лектор на это забивает
