# Stellar Burgers Ul: автоматизация тестирования на Java

Тестирование учебного проекта по автотестированию веб-прилождения Stellar Burgers в Google Chrome и Яндекс.Браузере.

## Документация
[Ссылка](https://stellarburgers.nomoreparties.site/) на учебное приложение Stellar Burgers.

## Описание

Версия Java 11.

В проекте используется библиотека:
- JUnit 4
- Selenium

## Инструкция для запуска тестов

Для запуска автотеста необходимо:

1. Склонируйте репозиторий на свой компьютер с помощью команды:

 ```sh
 git clone git@github.com:DianaRazyapova/stellar-burgers-web-automation.git
```

2. Запустите тесты с помощью команды:

```sh
mvn clean test
```

## Структура проекта
```bash
pom.xml
README.md
.gitignore
src
|-- main
|   |-- java
|   |   |-- client
|   |   |   |-- User.java
|   |   |   |-- UserClient.java
|   |   |-- page_object
|   |   |   |-- LoginPage.java
|   |   |   |-- MainPage.java
|   |   |   |-- ProfilePage.java
|   |   |   |-- RecoverPasswordPage.java
|   |   |   |-- RegisterPage.java
|-- test
|   |-- java
|   |   |-- tests
|   |   |   |-- LoginTest.java
|   |   |   |-- RegistrationTest.java
|   |   |   |-- TransitionsPersonalAccountTest.java
|   |   |   |-- TransitionsSectionsConstructorTest.java
```
## Выполненые задачи
1. Проверена регистрация:
- успешная регистрация;
- ошибка для некорректного пароля. Минимальный пароль — шесть символов.

2. Проверен вход:
- по кнопке «Войти в аккаунт» на главной;
- через кнопку «Личный кабинет»;
- через кнопку в форме регистрации;
- через кнопку в форме восстановления пароля.

3. Проверен переход в личный кабинет (по клику на «Личный кабинет»).


4. Проверен переход из личного кабинета в конструктор (по клику на «Конструктор» и на логотип Stellar Burgers).


5. Проверен выход из аккаунта.


6. Проверено, что работают переходы к разделам:
- «Булки»;
- «Соусы»;
- «Начинки».