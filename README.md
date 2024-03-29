#Дипломный Проект по автоматизации IBS


## 🚀: Содержание:

- [Технологии и инструменты](#earth_africa-технологии-и-инструменты)
- [Реализованные проверки](#earth_africa-Реализованные-проверки)
- [Сборка в Jenkins](#earth_africa-Jenkins-job)
- [Запуск из терминала](#earth_africa-Запуск-тестов-из-терминала)
- [Allure отчет](#earth_africa-Allure-отчет)
- [Интеграция с Allure TestOps](#-интеграция-с-allure-testops)
- [Отчет в Telegram](#earth_africa-Уведомление-в-Telegram-при-помощи-бота)
- [Пример запуска теста в Selenoid](#earth_africa-Примеры-видео-о-прохождении-тестов)

## 🧰: Технологии и инструменты

<p align="center">
<a href="https://www.jetbrains.com/idea/"><img src="image/logo/Idea.svg" width="50" height="50"  alt="IDEA"/></a>
<a href="https://www.java.com/"><img src="image/logo/Java.svg" width="50" height="50"  alt="Java"/></a>
<a href="https://github.com/"><img src="image/logo/GitHub.svg" width="50" height="50"  alt="Github"/></a>
<a href="https://junit.org/junit5/"><img src="image/logo/Junit5.svg" width="50" height="50"  alt="JUnit 5"/></a>
<a href="https://gradle.org/"><img src="image/logo/Gradle.svg" width="50" height="50"  alt="Gradle"/></a>
<a href="https://selenide.org/"><img src="image/logo/Selenide.svg" width="50" height="50"  alt="Selenide"/></a>
<a href="https://aerokube.com/selenoid/"><img src="image/logo/Selenoid.svg" width="50" height="50"  alt="Selenoid"/></a>
<a href="https://github.com/allure-framework/allure2"><img src="image/logo/Allure.svg" width="50" height="50"  alt="Allure"/></a>
<a href="https://www.jenkins.io/"><img src="image/logo/Jenkins.svg" width="50" height="50"  alt="Jenkins"/></a>
</p>

## ⚓: Реализованные проверки

 Тест 1
- ✓ Открыть русскую версию сайта ibs.ru
- ✓ Нажать на кнопку "Принять условия" (cookie)

 Тест 2
- ✓ Нажать поиск
- ✓ Выбрать "Импортозамещение"
- ✓ Проверить что отображаются результаты

 Тест 3
- ✓ Выполнить поиск компании IBS
- ✓ Проверить что в названии присутствует текст "IBS — ведущая российская IT-сервисная компания"


## <img src="image/logo/Jenkins.svg" width="25" height="25"  alt="Jenkins"/></a> Jenkins <a target="_blank" href="https://jenkins.autotests.cloud/job/valekseevUI/"> job </a>
<p align="center">
<a href="https://jenkins.autotests.cloud/job/valekseevUI/"> <img src="image/Jenkins01.jpg" alt="Jenkins"/></a>
</p>


## 🧙: Сборка в Jenkins:

- Browser (браузер, по умолчанию chrome)
- Version (версия браузера, по умолчанию 108.0)
- Browser_size (размер окна браузера, по умолчанию 1920x1080)



## 🏗️: Запуск тестов из терминала
Локальный запуск:
```
gradle clean test
```

Удаленный запуск:
```
clean
test
-Dbrowser=${BROWSER}
-Dversion=${VERSION}
-Dsize=${BROWSER_SIZE}
-Durl=${REMOTE_URL}
```

## <img src="image/logo/Allure.svg" width="25" height="25"  alt="Allure"/></a> Отчет в <a target="_blank" href="https://jenkins.autotests.cloud/job/valekseevUI">Allure report</a>

## 🧪: Тесты
<p align="center">
<img title="Allure Tests" src="image/Test.png">
</p>

## ⛅: Основной отчет
<p align="center">
<img title="Allure Overview Dashboard" src="image/report.jpg">
</p>

## 💹: Графики
<p align="center">
<img title="Allure Tests" src="image/graff.png">
</p>

## <img width="4%" title="Allure TestOPS" src="image/logo/Allure.svg"> Интеграция с [Allure TestOps](https://allure.autotests.cloud/launch/20548)
<p align="center">
<img title="Allure Tests" src="image/Test.png">
</p>

##   Отчет в Telegram
После завершения сборки специальный бот, созданный в <code>Telegram</code>, автоматически обрабатывает и отправляет сообщение с отчетом о прогоне тестов.

<p align="center">
<img title="Telegram Notifications" src="image/notification22.jpg">

## <img width="4%" title="Selenoid" src="image/logo/Selenoid.svg"> Пример запуска теста в Selenoid

> Видео примеры запуска тестов
<p align="center">
  <img title="Selenoid Video" src="image/video/video.gif">
</p>
