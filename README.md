# Курс Яндекс.Практикума «Архитектура ПО»

## Практическая работа спринта № 5

### Лог Rasa

Лог-файл диалога с чатботом — это файл `ai/rasa.log`. Лог сделан во время сеанса общения через web-UI.

### Запустить

Если есть желание проверить работу чат-бота, то после клонирования проекта следует:

* создать виртуальное окружение Python версии 3.10;

* с помощью pip установить туда rasa и transformers;

* выполнить следующие команды (вместо N укажите количество потоков, обычно, столько, сколько ядер имеет CPU):

```bash
$ cd ai
$ time rasa train --quiet --num-threads N
$ rasa shell -vv
```
