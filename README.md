# Дипломная работа по курсу "Инженер по тестированию: с нуля до middle" в Нетологии

## Тестирование мобильного приложение "Хоспис"
[Задание](https://github.com/netology-code/qamid-diplom)

### Процедура запуска тестов и создание allure-отчета
- Склонировать репозиторий
- Открыть проект в Android Studio
- Скомпилировать проект
- Запустить эмуляторр на Android API 29 (Pixel 2).
- Для запуска тестов во вкладке Run нажать: Run 'Tests in 'ru.iteco.fmhandroid.ui.tests"
- После выполнения всех тестов, выгрузить каталог SDCARD/googletest/test_outputfiles/allure-results с эмулятора (при помощи Device Explorer) в папку allure-results
- Выполнить в терминале команду allure serve
