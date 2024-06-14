# Пример использования GreenAPI

Этот проект демонстрирует использование API GreenAPI для работы с мессенджером WhatsApp.

## Инструкции по запуску

1. **Установка**
   - Склонируйте репозиторий на локальную машину:
     ```
     git clone https://github.com/Fzysx/green-api-test.git
     ```
   - Перейдите в директорию проекта:
     ```
     cd green-api-test
     ```

2. **Настройка**
   - Откройте файл `index.html` в любом текстовом редакторе.
   - Замените значение `apiUrl` на ваше значения от GreenAPI. Указано в личном кабинете https://console.green-api.com/instanceList -> [Выбрать инстанс] -> поле 'apiUrl'.

3. **Запуск**
   - Откройте файл `index.html` в браузере.

## Примеры использования

### Получение настроек

- Введите `idInstance` и `apiTokenInstance`. Значения указаны в инстансе в личном кабинете в полях 'idInstance' и 'apiTokenInstance'
- Нажмите кнопку `getSettings`.
- Ожидайте ответа API, который отобразится в поле `Ответ`. (https://green-api.com/docs/api/account/GetSettings/)

### Получение состояния аккаунта
- Введите `idInstance` и `apiTokenInstance`. Значения указаны в инстансе в личном кабинете в полях 'idInstance' и 'apiTokenInstance'
- Нажмите кнопку `getStateInstance`.
- Ожидайте ответа API, который отобразится в поле `Ответ`. (https://green-api.com/docs/api/account/GetStateInstance/)

### Отправка сообщения

- Введите `idInstance`, `apiTokenInstance`, `chatId` и `message`. chatId - нужно указать номер телефона, к которому привязан WhatsApp адресата.
- Нажмите кнопку `sendMessage`.
- Ожидайте подтверждение отправки и ответ API в поле `Ответ`. (https://green-api.com/docs/api/sending/SendMessage/)

### Отправка файла по URL

- Введите `idInstance`, `apiTokenInstance`, `chatId` и `fileUrl`. `fileUrl` в формате 'https://my.site.com/img/horse.png'
- Нажмите кнопку `sendFileByUrl`.
- Ожидайте подтверждение отправки файла и ответ API в поле `Ответ`. (https://green-api.com/docs/api/sending/SendFileByUrl/)
