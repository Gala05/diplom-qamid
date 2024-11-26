# План по проверке и автоматизации мобильного приложения Хоспис

## Описание объекта тестирования

Приложение даёт функционал по работе с новостями хосписа и включает в себя:

- информацию о новостях и функционал для работы с ними;
- тематические цитаты;
- информацию о приложении.

## Список функций и описание системы

1.  При входе в приложение splash screen.
2.  Страница авторизации с полями ввода для логина и пароля. Кнопка "Войти".
3.  На главном экране (раздел "Главная")
    - appbar. Содержит
      - иконку навигации с перечнем перехода по разделам приложения Главная, Новости, О приложении
      - заголовок
      - иконка "Главное - жить любя" для просмотра тематических цитат
      - иконка для последующего выхода из приложения
    - Раздел Новости с разворотом и переходом на просмотр всех новостей (ВСЕ НОВОСТИ). Новость включает в себя поля: Категория (объявление, день рождения, зарплата, профсоюз, праздник, массаж, благодарность, нужна помощь), Заголовок, Дата публикации, Время публикации, Описание, чек-бокс Active/Not active.
4.  Раздел "Новости" содержит

    - заголовок и navigation bar с кнопками
      - сортировки новости по дате публикации
      - фильтрации новостей по категории или дате публикации
      - редактирования новости.
    - текстовые блоки с опубликованными новостями с возможностью свернуть/развернуть.

    При нажатии кнопки для редактирования новости выходит окно, которое содержит

    - заголовок и navigation bar с кнопками
      - сортировки новостей по дате публикации
      - фильтрации новостей по категории или дате публикации
      - добавление/удаление новости. При добавлении новости необходимо заполнить поля и нажать кнопку "Сохранить" для сохранения, или "Закрыть" для выхода из режима добавления.
    - текстовые блоки с новостями. Содержат в себе названиее, дату публикации, дата создания, автор. Также на текстовом блоке есть кнопки удалить, редактировать и свернуть/развернуть, а также сведения об активации.

5.  Раздел "О приложении". Отображается версия, а также две ссылки на Privacy policy (политика конфиденциальности) и Terms of use (пользовательское соглашение).

## Последовательность проведения работ

1. Составление плана
2. Составление чек-листа
3. Составление тест-кейсов
4. Ручное тестирование
5. Автоматизация проверки приложения.
6. Составление отчета о тестировании

## Критерий начала тестирования

Приложение можно установить на эмулятор. Оно открывается.

## Критерий окончания тестирования

Проведены все запланированные тесты, получены отчеты.

## Интервальная оценка, необходимая для проведения тестирования и автоматизации, с учётом рисков (в часах)

1. Подготовительный этап  
   Настройка окружения (установка и настройка Android Studio, эмулятора, инструментов) - 1 (с учетом рисков - 2)
2. Разработка документации  
   Написание тестовых сценариев (чек-листов и тест-кейсов) - 7 (с учетом рисков - 9)
3. Проведение тестирования  
   Ручное тестирование - 2 (с учетом рисков - 3)
4. Автоматизация тестирования  
   Автоматизация тестирования с помощью Espresso/UI Automator - 90 (с учетом рисков - 110)
5. Отчетность  
   Подключение Allure и составление отчетности - 1 (с учетом рисков - 2)

## Стратегия тестирования (виды тестирования)

Ручное  
Автоматизированное

### Автоматизация следующих тест-кейсов (id, название кейса в файле Cases.xls)

1 Авторизация зарегистрированного пользователя приложения  
2 Авторизация незарегистрированного пользователя приложения  
3 Авторизация с неверным логином и верным паролем  
4 Авторизация с верным логином и неверным паролем  
5 Авторизация с пустыми полями  
6 Авторизация пользователя при использовании в поле логина SQL инъекции  
7 Авторизация пользователя при использовании в поле пароля SQL инъекции  
8 Навигация по разделам  
9 Сворачивание и разворачивание общего списка "Новости" в разделе "Главная"  
10 На главной странице приложения нажатие кнопки "ВСЕ НОВОСТИ" и переход в раздел "Новости"  
11 Чтение новости в разделе "Главная"  
14 Сортировка новостей в разделе "Новости"  
15 Чтение новости в разделе "Новости"  
17 Сортировка новостей в режиме редактирования новостей раздела "Новости"  
18 Удаление новости в режиме редактирования новостей раздела "Новости"  
19 Редактирование новости в режиме редактирования новостей раздела "Новости"  
20 Добавление новости с заполненными полями  
21 Добавление новости с незаполненными обязательными пустыми полями  
22 Фильтрация новостей по категории в разделе "Новости"  
23 Фильтрация новостей по дате публикации в разделе "Новости"  
24 Фильтрация новостей по категории в режиме редактирования в разделе "Новости"  
25 Фильтрация новостей по дате публикации в режиме редактирования в разделе "Новости"  
27 Чтение цитаты в разделе "Главное - жить любя"  
28 Переход по ссылке Privacy Policy в разделе "О приложении"  
29 Переход по ссылке Terms of use в разделе "О приложении"  
30 Выход из приложения

### Ручное тестирование следующих тест-кейсов (id, название кейса в файле Cases.xls)

12 Проверка Pull to refresh раздела "Главная"  
13 Скролл новостей в разделе"Новости"  
16 Проверка Pull to refresh раздела "Новости"  
26 Скролл цитат в разделе "Главное - жить любя"  
31 Работа приложения на светлой теме устройства  
32 Работа приложения на темной теме устройства  
33 Работа приложения при альбомной ориентации экрана устройства  
34 Соответствие языка интерфейса приложения языку устройства  
35 Восстановление работы приложения после сворачивания  
36 Восстановление работы приложения после прерывания  
37 Уведомление о наличии входящего звонка  
38 Уведомление о поступившем SMS сообщении  
39 Работа приложения при использовании сети 2G  
40 Работа приложения при использовании сети 3G  
41 Работа приложения при отсутствии сети Интернет на мобильном устройстве

## Устройство-эмулятор мобильного устройства

Pixel 2 API 29, Android 10

## Перечень используемых инструментов

1. Git-hub - веб-сервис для облачного хранения кода и и совместной командной разработки.
2. Android Studio - интегрированная среда разработки с помощью которой становятся доступны инструменты для создания и тестирования приложений на платформе Android OS.
3. Java - язык программирования для написания автотестов.
4. UI Automator - библиотека API для взаимодействия с элементами пользовательского интерфейса, которые видны на экране в любой момент времени. UI Automator позволяет автоматизировать тесты, которые взаимодействуют с пользовательским интерфейсом приложения Android, и проверять, что приложение ведет себя так, как ожидается.
5. Espresso - это тестовый фреймворк для выполнения сложных тестов пользовательского интерфейса.
6. Allure - инструмент для создания отчетов о тестировании, который помогает визуализировать результаты тестов.