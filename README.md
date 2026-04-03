#  GREEN-API Test Client

Веб-приложение для тестирования методов **[GREEN-API](https://green-api.com/)** — отправка сообщений и файлов через WhatsApp, получение настроек и состояния инстанса.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![GREEN-API](https://img.shields.io/badge/GREEN--API-00A884?style=flat&logo=whatsapp&logoColor=white)

---

## Демо

**Живая страница:** [https://eenclaver.github.io/GREEN-API-Test-Client/] 
---

## Функциональность

Реализованы **4 основных метода** GREEN-API:

| Метод | Описание |
|-------|----------|
| `getSettings` | Получение настроек текущего инстанса |
| `getStateInstance` | Проверка состояния инстанса (авторизован / нет) |
| `sendMessage` | Отправка текстового сообщения на номер WhatsApp |
| `sendFileByUrl` | Отправка файла (изображение, документ, аудио) по прямой ссылке |

### Дополнительные возможности

- Ручной ввод `idInstance` и `ApiTokenInstance`
- Автосохранение введённых данных в `localStorage`
- Поле вывода ответов API (только для чтения) с временными метками
- Очистка лога одной кнопкой
- Адаптивный дизайн для мобильных устройств

---

## Как использовать

### 1. Получить учётные данные GREEN-API

1. Зарегистрируйтесь на [GREEN-API](https://green-api.com/)
2. Создайте бесплатный инстанс в личном кабинете
3. Отсканируйте QR-код через WhatsApp (на телефоне: «Связанные устройства» → «Привязать устройство»)
4. Скопируйте `idInstance` и `ApiTokenInstance` из настроек инстанса

### 2. Открыть страницу

- Локально: скачайте `index.html` и откройте в браузере
- Онлайн: перейдите по [https://eenclaver.github.io/GREEN-API-Test-Client/]

### 3. Ввести данные и тестировать

- Вставьте `idInstance` и `ApiTokenInstance` в соответствующие поля
- Нажмите `getSettings` или `getStateInstance` — ответ появится внизу
- Для отправки сообщения:
  - Введите номер получателя в формате `79991234567` (без +)
  - Напишите текст → `sendMessage`
- Для отправки файла по ссылке:
  - Укажите номер получателя, прямую ссылку на файл и (опционально) имя файла
  - Нажмите `sendFileByUrl`

> **Важно:** Номер телефона должен быть зарегистрирован в WhatsApp и авторизован в инстансе.

---

## Структура проекта

  greenapi-test-client/  <br />
  ├── index.html # HTML-страница <br /> 
  └── README.md # Документация <br />
---

## Используемые технологии

- **HTML5** — семантическая разметка
- **CSS3** — Flexbox, градиенты, адаптив
- **JavaScript (ES6+)** — Fetch API, async/await, работа с localStorage
- **GREEN-API REST API** — официальные методы

---

## Установка и запуск локально

```bash
git clone https://github.com/Eenclaver/GREEN-API-Test-Client.git
cd GREEN-API-Test-Client
# Открыть index.html в браузере
```
