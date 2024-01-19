# Проект по UI автоматизации тестирования магазина компьютерных игры [STEAM](https://store.steampowered.com/) 




![UUZEtqRIObvUmrG3_noHRg.jpeg](picturies%2FUUZEtqRIObvUmrG3_noHRg.jpeg)



## 📝 Описание проекта 
Данный проект является дипломной работай курса по автоматизационному тестированию от [QA_Guru](https://qa.guru/?utm_source=yandex&utm_medium=cpc&utm_campaign=Search%2FBrand&utm_content=type1.1.premium.13541539116.desktop...none.search.Смоленск&utm_term=qa%20guru&yclid=11201726552105025535). 
Данный проект реализован под локальное и удаленное развертывание и запуск авто-тестов. 

Проект находиться в открытом доступе и его  можно использовать в качестве шаблона для ваших целей, кастомизации и т.п.

Ваш лайк в качестве звездочки ⭐️ поставленной этому проекту - одобряется и ни как не запрещается ) 



##  ✏️ Список автоматизированных тест-кейсов:
- [x] _Добавление игры в  корзину_
- [x] _Удаление игры из корзины_ 
- [x] _Удаление нескольких игр из корзины_
- [x] _Проверка соответствия описания игры_  
- [x] _Проверка работы поиковой выдачи _**Steam**__
- [x] _Проверка отображения текста при смене языка_ 
- [x] _Поиск друзей в _**Steam**_ во вкладке **Community**_



## 🧰 Используемые технологии и инструменты:
| Java                                                                                                      | IntelliJ Idea                                                                                                                 | GitHub                                                                                                     | JUnit 5                                                                                                           | Gradle                                                                                                     | Selenide                                                                                                         | Selenoid                                                                                                                  |  Jenkins                                                                                                           |
|:----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------:|
| <a href="https://www.java.com/"><img alt="Java" height="50" src="picturies/Java.svg" width="50"/></a>  | <a id ="tech" href="https://www.jetbrains.com/idea/"><img alt="IDEA" height="50" src="picturies/Idea.svg" width="50"/></a> | <a href="https://github.com/"><img alt="Github" height="50" src="picturies/GitHub.svg" width="50"/></a> | <a href="https://junit.org/junit5/"><img alt="JUnit 5" height="50" src="picturies/Junit5.svg" width="50"/></a> | <a href="https://gradle.org/"><img alt="Gradle" height="50" src="picturies/Gradle.svg" width="50"/></a> | <a href="https://selenide.org/"><img alt="Selenide" height="50" src="picturies/Selenide.svg" width="50"/></a> | <a href="https://aerokube.com/selenoid/"><img alt="Selenoid" height="50" src="picturies/Selenoid.svg" width="50"/></a> |   <a href="https://www.jenkins.io/"><img alt="Jenkins" height="50" src="picturies/Jenkins.svg" width="50"/></a> |


| Allure                                                                                                                     |
|----------------------------------------------------------------------------------------------------------------------------|
| <a href="https://github.com/allure-framework"><img alt="Allure" height="50" src="picturies/Allure.svg" width="50"/></a> |


###  💻 Выполнить запуск автотестов из терминала можно командой:  

`gradle clean test`

### Удаленный запуск тестов:

```bash
gradle clean test

-Dbrowser=${browser}
-DbrowserVersion=${browserVersion}
-DbrowserSize=${browserSize}
-DremoteUrl=${remoteUrl}
-DremoteUrl=${TASK}
```

### Параметры запуска тестов:
```browser``` - браузер в котором будут выполняться авто-тесты (по умолчанию ```chrome```)

```browserSize``` - размер окна браузера (по умолчанию - ```1920x1080```)

```browserVersion``` - версия браузера (по умолчанию ```100.0```)

```remoteUrl``` - адрес удаленного сервера, где будут запускаться авто-тесты

```task``` - отдельные группы авто-тестов которые нужно запустить

### Запуск авто-тестов в [Jenkins](https://jenkins.autotests.cloud/job/C27-mateenkov-General-UI/)
**Главная страница проекта:**
![img.png](picturies/GenJenkins.png)

Для запуска сборки необходимо указать значения параметров и нажать кнопку ```Build with Parameters```

**Страница настройки параметров:**
![img.png](picturies/JenkinsParametersPage.png)

После натсройи парамметров, запустить сборку можно по кнопке ```Build```

Результаты сборки можно посмотреть в Allure отчёте, кликнув на значок ![img.png](picturies/iconAllure.png) ```Allure Report```.

### Отчет о результатах проведенных авто-тестов в [Allure Report](https://jenkins.autotests.cloud/job/C27-mateenkov-General-UI/7/allure/)

**Главная страница Allure Report:**
![img.png](picturies/genPageAllureReport.png)

**Авто-тесты с шагами воспроизведения:**
![img.png](picturies/tests.png)

**Графики с результатами тестирования:**
![img.png](picturies/graphic.png)

### Отчет о выполнении тестов в Telegram с использованием бота:
**Оповещения о результатах сборки проекта:**

![img.png](picturies/telegramReporting.png)

### Пример запуска авто-теста в Selenoid

В конце каждого авто-теста выполняется скриншот и запись экрана, и прикрепляется к каждому тесту в Allure  отчете 

Запись экрана авто-теста - ```Добавление игры в корзину``` 

![addItemToCart.gif](video%2FaddItemToCart.gif)