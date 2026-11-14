# Видеоплеер ГОСТФильм

Прототип видеоплеера для урока Devman «Верстаем видеоплеер».

[Открыть плеер](https://Arrrtemka246.github.io/devman-video-player/).

Работают запуск и пауза, выключение и включение звука, полноэкранный просмотр.
Плеер растягивает видео через Flexbox, оставляя место панели управления;
размеры внешнего контейнера задаются в классе `video-player`. JS-классы служат
подключению библиотеки, отдельные CSS-классы — оформлению.

## Локальный запуск

Нужен Python 3.10 или новее.

```sh
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
livereload --host 127.0.0.1 -p 8012 .
```

Откройте http://127.0.0.1:8012/. Livereload сам обновляет страницу после
изменения HTML и CSS. Для остановки нажмите Ctrl+C.

Дополнительные упражнения урока: [HTML](examples/search.html) и
[Flexbox](examples/flex.html).

## Публикация

В настройках репозитория GitHub откройте **Pages**, выберите раздачу из ветки
`main`, папка `/ (root)`, и сохраните. После сборки сайт доступен по ссылке выше.
Ссылки на локальные ресурсы относительные, поэтому проект работает в подкаталоге
GitHub Pages. Тестовое видео загружается с учебного сайта Devman.

## Проверки

В Safari проверены запуск, пауза, смена кнопок звука, полноэкранный режим
и автоматическое обновление livereload. HTML проверяется W3C Nu Validator.

## Источники

- [Учебная библиотека Devman](https://github.com/devmanorg/video-player-jslib) — `player.js`.
- [jQuery 3.4.1](https://jquery.com/) и [Playable 2.10.3](https://github.com/wix/playable).
- [Font Awesome 4.7](https://fontawesome.com/v4/) — иконки.

Зависимости для браузера лежат в `vendor/`. Учебный проект [Devman](https://dvmn.org/).
