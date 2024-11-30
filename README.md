Подключите свой агент ngrok к учётной записи ngrok. Если ещё не сделали, зарегистрируйтесь на сайте https://ngrok.com и скачайте приложение с официального сайта для Windows: https://download.ngrok.com/windows.

Скопируйте ваш аутентификационный токен ngrok.

Выполните следующую команду в терминале, чтобы установить Authtoken:

```bash
ngrok config add-authtoken <ваш_токен>
```

Перейдите на страницу «Настройка и установка» в Панели управления для получения специфической команды конфигурации вашей учётной записи.

Запустите ngrok, выполнив следующую команду:

```bash
ngrok.exe http 8360 (localhost на порту 8360)
```

В терминале появится интерфейс консоли с информацией о запущенном туннеле.

После этого загрузите ZIP-архив проекта. В распакованной папке найдите файл index.html.

После этого проверьте, что у вас установлена версия Python выше 3.9 (не так критично).
В новом окне терминала (у вас будет два окна: одно с ngrok, второе — с хостингом сайта) выполните команду:

```bash
python -m http.server -cgi 8360
```

После этого скопируйте ссылку из терминала с запущенным сервисом Ngrok, вставьте её в поисковую строку любого браузера и наслаждайтесь игрой. Маджонг от команды ITL10).
Приятного использования!
