# Создание сервера {{ metastore-name }}

{% list tabs %}

- Консоль управления

  1. В [консоли управления]({{ link-console-main }}) выберите каталог, в котором нужно создать сервер.
  1. Нажмите кнопку **Создать ресурс** и выберите ![image](../../../_assets/data-proc/data-proc.svg) **Кластер {{ dataproc-name }}** в выпадающем списке.
  1. На левой панели нажмите на значок ![image](../../../_assets/data-proc/metastore.svg) **Metastore-сервер**.
  1. Нажмите кнопку **Создать кластер**.
  1. Введите имя сервера в поле **Имя кластера**. Имя должно быть уникальным в рамках каталога.
  1. В выпадающем списке выберите версию {{ metastore-name }}.
  1. Укажите минимальное и максимальное количество серверов {{ metastore-name }} на зону доступности.
  1. В блоке **Сетевые настройки** выберите сеть и подсеть, в которых будет размещен сервер {{ metastore-name }}.
  1. При необходимости активируйте защиту сервера от непреднамеренного удаления пользователем.

      Включенная защита не помешает подключиться к серверу вручную и удалить данные.

  1. Нажмите кнопку **Создать**.

{% endlist %}
