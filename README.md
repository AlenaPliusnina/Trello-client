Это мой консольный клиент для Trello!

Для работы приложения в файле trello.py необходимо заполнить поля key, token, board_id своими значениями, для этого:

   - нужно зарегистрироваться на сайте trello.com
   
   - перейти на trello.com/app-key, согласиться с условиями пользования и нажать "Показать API ключ" и добавить вместо key в файле trello.py
   
   - на той же странице перейти по ссылке на слове токен, отобразить его, cкопировать и добавить вместо token в файле trello.py
   
   - board_id можно полусить из адреса страницы с вашей доской trello, например для данного адреса https://trello.com/b/3MxML0oO/******, board_id = 3MxML0o 

Консольные команды для работы с приложением:
1. Чтобы отобразить все колонки и задачи в них - python trello.py
2. Добавить новую задачу в колонку: python trello.py create "name" "column_name" (где name - название задачи, column_name - название колонки)
3. Создать новую калонку: python trello.py add_column "column_name"  (где column_name - название колонки)
4. Переместить задачу из одной колонки в другую: python trello.py move "name" "column_name" (где name - название задачи которую хотите пернести, column_name - название колонки в которую будет перенесена задача)

Пример работы с приложением:

Интерфейс доски на сайте trello выглядит следующим образом:

![Интерфейс доски trello](https://github.com/AlenaPliusnina/Trello-client/blob/master/screenshots/screen_1.png)

Для того чтобы получить ту же информацию о задачах в консоли необходимо выполнить команду: python trello.py

![Получение задач trello в консоли](https://github.com/AlenaPliusnina/Trello-client/blob/master/screenshots/screen_2.png)

Добавление новой задачи через консоль показано на скриншоте ниже (добавляем задачу "test" в карточку "Спорт")

![Добавление новой задачи trello в консоли](https://github.com/AlenaPliusnina/Trello-client/blob/master/screenshots/screen_3.png)

При этом данные на сайте trello также обновляются

![Добавление новой задачи trello на сайте](https://github.com/AlenaPliusnina/Trello-client/blob/master/screenshots/screen_4.png)

Также при помощи консольной команды можно перенести задачу в другую колонку/карточку (переносим задачу "test" в карточку "Домашние дела")

![Перенос задачи trello в консоли](https://github.com/AlenaPliusnina/Trello-client/blob/master/screenshots/screen_5.png)

В результате чего данные на сайте буду обновлены 

![Перенос задачи trello на сайте](https://github.com/AlenaPliusnina/Trello-client/blob/master/screenshots/screen_6.png)

    *** Обратите внимание на цифру рядом с названием карточки с группой задач, она обозночает колличество задач в этой группе, и также обновляется при изменении их колличества и обновлении данных через консоль.
