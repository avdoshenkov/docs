# Metrics Collector

Приложение по таймеру собирает информацию об использовании ресурсов {{ yandex-cloud }} и записывает полученные значения в сервис [{{ monitoring-full-name }}](../monitoring).

## Необходимые платные ресурсы

В стоимость ресурсов для приложения входит плата за количество вызовов функции, вычислительные ресурсы, выделенные для выполнения функции, и исходящий трафик (см. [тарифы {{ sf-full-name }}](../functions/pricing.md)).

## Разверните приложение

1. В [консоли управления]({{ link-console-main }}) выберите каталог, в котором хотите развернуть приложение.
1. Выберите сервис **{{ cloud-apps-name }}**.
1. На панели слева выберите **Магазин приложений**.
1. Выберите **Metrics Collector** и нажмите кнопку **Использовать**.
1. Укажите:
    * Имя приложения.
    * (опционально) Описание приложения.
    * Сервисный аккаунт с ролью `admin` на каталог или выберите **Автоматически**, чтобы нужный сервисный аккаунт создался при установке приложения. От имени этого сервисного аккаунта будут создаваться ресурсы приложения.
1. Нажмите кнопку **Установить** и дождитесь, пока приложение установится.
