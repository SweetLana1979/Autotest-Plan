### План автоматизации тестирования сценария перехода к форме записи и заполнения формы записи ###

**Сценарии навигации по странице для перехода к форме записи**

_Сценарий 01 Переход через Направление Обучения_

1. Зайти в браузере на главную страницу сайта «Нетологии» (netology.ru)
2. В разделе «Направление обучения» выбрать «Программирование», кликнуть
3. На открывшейся странице с перечнем курсов выбрать «Тестировщик ПО», кликнуть
4. На открывшейся странице курса «Тестировщик» кликнуть по кнопке «Записаться»
5. После нажатия кнопки откроется форма записи

_Сценарий 02 Переход через Каталог Курсов_

1. Зайти в браузере на главную страницу сайта «Нетологии» (netology.ru)
2. Нажать на меню «Каталог курсов»
3. В открывшемся меню выбрать «Программирование», кликнуть
4. На открывшейся странице с перечнем курсов выбрать «Тестировщик ПО», кликнуть
5. На открывшейся странице курса «Тестировщик» кликнуть по кнопке «Записаться»
6. После нажатия кнопки откроется форма записи

_Сценарий 03 Переход через Каталог Курсов\_Строка поиска_

1. Зайти в браузере на главную страницу сайта «Нетологии» (netology.ru)
2. Нажать на меню «Каталог курсов»
3. В поисковой строке «Какой курс вам нужен?» ввести слово «Тестировщик», нажать кнопку «Найти курс»
4. В открывшемся меню выбрать «Тестировщик ПО», кликнуть
5. На открывшейся странице курса «Тестировщик» кликнуть по кнопке «Записаться»
6. После нажатия кнопки откроется форма записи

_Сценарий 04 Переход через футер_

1. Зайти в браузере на главную страницу сайта «Нетологии» (netology.ru)
2. Пролистать главную страницу до футера сайта, выбрать раздел «Обучение», нажать на «Программирование»
3. На открывшейся странице с перечнем курсов выбрать «Тестировщик ПО», кликнуть
4. На открывшейся странице курса «Тестировщик» кликнуть по кнопке «Записаться»
5. После нажатия кнопки откроется форма записи


**Сценарии заполнения формы и отправки**

_Сценарий 01. Отправка формы с валидными данными_

1. Зайти на страницу с формой записи на курс "Тестировщик ПО"
2. Заполнить поля формы валидными данными:
   Имя: Иван
   Телефон: +79999999999
   Эл.почта: netology@mail.ru
3. Нажать кнопку «Записаться»
   Ожидаемый результат: отобразится сообщение об успешной записи на курс

_Сценарий 02. Отправка формы с невалидным именем_

1. Зайти на страницу с формой записи на курс "Тестировщик ПО"
2. Ввести в поле «Имя» спецсимволы (& @ $) или цифры (555)
   Ожидаемый результат: отобразится сообщение «Должно состоять из букв»

_Сценарий 03. Отправка формы с невалидным форматом телефона_

1. Зайти на страницу с формой записи на курс "Тестировщик ПО".
2. Ввести в поле «Телефон» невалидные данные (39999999999)
   Ожидаемый результат: отобразится сообщение «Номер в формате +7 (999) 999-99-99»

_Сценарий 04. Отправка формы с невалидным номером телефона_

1. Зайти на страницу с формой записи на курс "Тестировщик ПО"
2. Ввести в поле «Телефон» нули
   Ожидаемый результат: отобразится сообщение «Номер в формате +7 (999) 999-99-99»

_Сценарий 05. Отправка формы с пустым полем Телефон_

1. Зайти на страницу с формой записи на курс "Тестировщик ПО"
2. Оставить поле «Телефон» пустым
   Ожидаемый результат: под полем отобразится сообщение «Обязательное поле»

_Сценарий 06. Отправка формы с пустым полем Имя_

1. Зайти на страницу с формой записи на курс "Тестировщик ПО"
2. Оставить поле «Имя» пустым
   Ожидаемый результат: под полем отобразится сообщение «Обязательное поле»

_Сценарий 07. Отправка формы с невалидным эл.адресом_

1. Зайти на страницу с формой записи на курс "Тестировщик ПО"
2. Ввести в поле «Электронная почта» невалидные данные (netologymail.ru)
   Ожидаемый результат: отобразится сообщение «Неверный email»

**Перечень инструментов**

- IntelliJ IDEA – редактор кода
- Selenide - библиотека для написания стабильных UI тестов с открытым исходным кодом (лаконичный синтаксис, автоматическое решение большинства проблем с Ajax, ожиданием и таймаутами, управление жизнедеятельностью браузера, автоматическое создание скриншотов)
- Maven — инструмент для автоматизации сборки проектов
- TestNG — тестовый фреймворк
- Allure - инструмент для создания отчетов о тестировании с открытым исходным кодом (обеспечивает прозрачность в процессе создания и выполнения функциональных тестов; красивые и понятные отчёты)
- Github - веб-сервис для хостинга IT-проектов и их совместной разработки

**Перечень необходимых разрешений, данных и доступов**

- Разрешение на автоматизированное тестирование у владельца сайта
- Доступ к базе данных, к API
- Спецификация на сайт

**Перечень и описание возможных рисков при автоматизации**

- Отсутствие тестовых меток при подборе селекторов
- Изменение кода, подключение новых патчей
- Сбой инфраструктуры

**Перечень необходимых специалистов для автоматизации**

- инженер автотестирования – 1 чел.

**Интервальная оценка с учётом рисков в часах**

- 24 часа (+5 часов на случай реализации риска).
