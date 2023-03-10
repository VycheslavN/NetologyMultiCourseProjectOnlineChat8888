# Курсовой проект "Сетевой чат"
(мое описание см ниже)
## Описание проекта
Вам нужно разработать два приложения для обмена текстовыми сообщениями по сети с помощью консоли (терминала) между двумя и более пользователями.

Первое приложение - сервер чата, должно ожидать подключения пользователей.

Второе приложение - клиент чата, подключается к серверу чата и осуществляет доставку и получение новых сообщений.

Все сообщения должны записываться в file.log как на сервере, так и на клиентах. File.log должен дополняться при каждом запуске, а также при отправленном или полученном сообщении. Выход из чата должен быть осуществлен по команде exit.

## Требования к серверу
Установка порта для подключения клиентов через файл настроек (например, settings.txt);
Возможность подключиться к серверу в любой момент и присоединиться к чату;
Отправка новых сообщений клиентам;
Запись всех отправленных через сервер сообщений с указанием имени пользователя и времени отправки.
## Требования к клиенту
Выбор имени для участия в чате;
Прочитать настройки приложения из файла настроек - например, номер порта сервера;
Подключение к указанному в настройках серверу;
Для выхода из чата нужно набрать команду выхода - “/exit”;
Каждое сообщение участников должно записываться в текстовый файл - файл логирования. При каждом запуске приложения файл должен дополняться.
## Требования в реализации
Сервер должен уметь одновременно ожидать новых пользователей и обрабатывать поступающие сообщения от пользователей;
Использован сборщик пакетов gradle/maven;
Код размещен на github;
Код покрыт unit-тестами.
## Шаги реализации:
Нарисовать схему приложений;
Описать архитектуру приложений (сколько потоков за что отвечают, придумать протокол обмена сообщениями между приложениями);
Создать репозиторий проекта на github;
Написать сервер;
Провести интеграционный тест сервера, например с помощью telnet;
Написать клиент;
Провести интеграционный тест сервера и клиента;
Протестировать сервер при подключении нескольких клиентов;
Написать README.md к проекту;
Отправить на проверку.

# Моё описание проекта
Разработал два приложения для обмена текстовыми сообщениями по сети с помощью консоли (терминала) между двумя и более пользователями.
Первое приложение - сервер чата, ожидает подключения пользователей.
Второе приложение - клиент чата, подключается к серверу чата и осуществляет доставку и получение новых сообщений.
Все сообщения, а также все исключительные ситуации, записываются в log.txt, который дополняется при каждом запуске, а также при отправленном или полученном сообщении, как на сервере, так и на клиентах. Выход из чата осуществляется по команде "/exit".
## Описание реализации
•	Сервер умеет одновременно ожидать новых пользователей и обрабатывать поступающие сообщения от пользователей;
•	В качестве файла настроек используется settings.properties;
•	Реализовано логирование, запись логов в файл log.txt;
•	Использован сборщик пакетов MAVEN;
•	Код размещен на github;
•	Код покрыт unit-тестами.
## Описание сервера
•	Порт для подключения клиентов устанавливается через файл настроек settings.properties;
•	Возможность подключиться к серверу в любой момент и присоединиться к чату;
•	Отправка новых сообщений клиентам;
•	Запись в log.txt всех отправленных через сервер сообщений с указанием имени пользователя и времени отправки.
## Описание клиента
•	Возможность выбора имени для участия в чате;
•	Чтение настройки приложения (порт и хост) из файла настроек settings.properties;
•	Подключение к указанному в настройках серверу;
•	Для выхода из чата нужно набрать команду выхода - “/exit”;
•	Каждое сообщение записывается в log.txt.

