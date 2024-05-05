# Домашнее задание к занятию «7.6. Cypress 1»

## Решения
* <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/cypress/e2e/booksApp/login.cy.js">login.cy.js</a> - автотесты авторизации.
* <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/cypress/e2e/booksApp/registeredUser.cy.js">registeredUser.cy.js</a> - автотесты залогиненного пользователя.
* <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/package.json">package.json</a> - с конфигурациями запуска автотестов.

<a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/tree/main/7.6">Репозиторий</a> с Cypress проектом.

## Что было сделано
* Создан <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/.gitignore">.gitignore</a>.
* Создан <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/package.json">package.json</a>
со скриптами запуска cypress с различными конфигурациями (браузеры, headless, разрешения экранов).
* Созданы конфигурационные файлы запуска cypress:
  * <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/cypress.config.js">cypress.config.js</a>,
  * <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/laptopView.config.js">laptopView.config.js</a>,
  * <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/mobileView.config.js">mobileView.config.js</a>.
* Создан служебный файл <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/cypress/support/commands.js">commands.js</a> с методами описывающими повторяющиеся операции взаимодействия с элементами.
* Реализованы классы с функциональными автотестами:
  * <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/cypress/e2e/booksApp/login.cy.js">login.cy.js</a>,
  * <a href="https://github.com/Nephedov/jsaqa-code-Nephedov93/blob/main/7.6/cypress/e2e/booksApp/registeredUser.cy.js">registeredUser.cy.js</a>.

## Описание Задания 1. Cypress. Установка и настройка проекта

1. Сделайте форк [проекта](https://github.com/netology-code/jsaqa-code/tree/main/booksApp) приложения для работы с книгами из лекции и запустите его локально на своей машине.
2. Мы можем тестировать логин и добавление книг.
3. Создайте новый проект для тестов на Cypress в отдельном репозитории.
4. Создайте spec-тест для ваших тестов.
5. Добавьте первый тест с проверкой отображения страницы.

  ### Добавление тестов

1. Повторите тесты, которые разбирали на лекции.
2. Добавьте 3 теста для проверки функциональности работы с книгами в избранном: выберите 3 наиболее важных теста.
3. Вынесите все повторяющиеся шаги в кастомные команды.
4. Не забывайте использовать настройки проекта для работы с базовым URL.
5. Запустите тесты. 


## Описание Задания 2. Настройка второй конфигурации

Cypress позволяет иметь несколько конфигураций для запуска. Вам нужно настроить их для своего проекта.

1. Добавьте вторую конфигурацию, используя [эту документацию](https://docs.cypress.io/guides/guides/environment-variables#Option-2-cypress-env-json).
2. В конфигурациях настройте параметры `view-port` для двух разных размеров экрана. Выберите самый популярный размер экрана на ноутбуках и на мобильных экранах.

## Описание Задания 3. Настройка скриптов запуска

Для упрощения работы с запуском тестов нужно настроить 4 скрипта для запуска в режимах headded и headless и разные браузеры для каждой из конфигураций.
