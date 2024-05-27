# Практика по дедупликации данных

Давайте представим, что вы работаете в отделе рисков крупного банка. Тогда на вашу работу влияют новости об окружающем мире и вам надо узнать о том какие это новости:
Позитивные/негативные;
Или узнать тематики, которые в них присутствуют.
У вас уже есть модели, которые решают эти задачи, но - БУМ! Новостей так много, что часто вы наблюдаете повторяющиеся новости, которые тратят ваше время и вы хотите избавиться от них и вместо этого попивать свой любимый лавандовый раф.

Именно такую задачу мы хотим решить

![best_guy](./images/gos_read_news.jpeg)

## Структура репозитория
- near_deduplication.ipynb: ноутбук для решения задачи дедубликации новостных данных;
- *.py - вспомогательные скрипты которые используются для решения задачи дедупликации (подробно расписано будет позже);
- train_set.csv, dev_set.csv - файлы для примеров;
- duplicated_news.csv - данные для самостоятельной работы;

На данный момент структура репозитория сырая. Будет изменяться.

## Как получить датасеты?

Для начала необходимы плагины для аутентификации:

```bash
pip install dvc[gdrive]
```

Далее просто введите

```bash
dvc pull
```
