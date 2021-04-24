# y-praktikum-slack-bot
slack bot for Yandex.Praktikum

## COMMANDS:

`/split-to-messages`

Разбивает куски текста, отделенные пустой строкой, на отдельные сообщения + добавляет меншены к каждому сообщению

Меншены нужно писать отдельной строкой (или строками), если хочется их продублировать в каждое сообщение

Пример:

```
/split-to-messages

Веселые истории
Экран покажет ваш

Веселые истории
В журнале

<link.to/website|Ералаш>

@Вася @Петя
@Катя


```

=>

```
Веселые истории
Экран покажет ваш

@Вася @Петя @Катя // как меншены здесь и ниже

// ----новое сообщение----

Веселые истории
В журнале

@Вася @Петя @Катя

// ----новое сообщение----

Ералаш // как ссылка

@Вася @Петя @Катя
```

## Deploy

https://slack.dev/bolt-js/deployments/heroku