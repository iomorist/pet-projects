# Telegram Bot для хранения кодов лабораторных работ

Привет! Я хочу рассказать о своем проекте - Telegram боте для хранения и управления кодами лабораторных работ. Этот бот стал моим решением проблемы организации и быстрого доступа к кодам различных лабораторных работ.

## Как появилась идея?

Во время учебы я часто сталкивался с необходимостью хранить и быстро находить коды различных лабораторных работ. Хранить их в отдельных файлах было неудобно, а поиск по папкам занимал много времени. Тогда я решил создать бота, который поможет организовать все коды в одном месте и обеспечит быстрый доступ к ним через Telegram.

## Что умеет бот?

Мой бот предоставляет следующие возможности:

- **Добавление кодов**: Пошаговый процесс добавления новой лабораторной работы, где вы указываете:
  - Название предмета
  - Номер лабораторной работы
  - Вариант
  - Сам код

- **Удобная навигация**: 
  - Просмотр всех предметов в виде кнопок
  - Выбор конкретного предмета для просмотра лабораторных работ
  - Быстрый доступ к коду любой лабораторной работы

- **Управление кодами**:
  - Редактирование существующих кодов
  - Удаление ненужных лабораторных работ
  - Автоматическая нумерация для удобной навигации

## Как это работает?

Бот построен на Python с использованием библиотеки python-telegram-bot. Для хранения данных я использовал SQLite, что обеспечивает надежное и быстрое хранение всех кодов. Интерфейс реализован с помощью интерактивных кнопок Telegram, что делает взаимодействие с ботом максимально удобным.

## Как использовать бота?

1. **Начало работы**:
   - Отправьте команду `/start`
   - Бот поприветствует вас и покажет список доступных команд

2. **Добавление новой лабораторной**:
   - Используйте команду `/add`
   - Следуйте инструкциям бота, вводя последовательно:
     - Название предмета
     - Номер лабораторной
     - Вариант
     - Код

3. **Просмотр кодов**:
   - Команда `/list` покажет все предметы
   - Выберите нужный предмет
   - Выберите конкретную лабораторную работу
   - Просматривайте код

4. **Управление кодами**:
   - `/edit <номер> <новый_код>` - для редактирования
   - `/delete <номер>` - для удаления
   - `/cancel` - для отмены текущего действия

## Технические детали

- **Язык программирования**: Python
- **Основные библиотеки**:
  - python-telegram-bot
  - sqlite3
  - python-dotenv
- **База данных**: SQLite
- **Структура данных**: Таблица с полями для предмета, номера лабораторной, варианта и кода

## Установка и запуск

1. Клонируйте репозиторий:
   ```bash
   git clone [URL репозитория]
   ```

2. Установите зависимости:
   ```bash
   pip install -r requirements.txt
   ```

3. Создайте файл `.env` и добавьте в него токен вашего бота:
   ```
   TELEGRAM_BOT_TOKEN=ваш_токен
   ```

4. Запустите бота:
   ```bash
   python bot.py
   ```

## Заключение

Этот бот стал для меня отличным проектом, где я смог применить свои знания Python и работы с API Telegram. Он не только решает практическую задачу организации кодов лабораторных работ, но и демонстрирует мои навыки в разработке пользовательских интерфейсов и работе с базами данных.

Я постоянно улучшаю бота, добавляя новые функции и оптимизируя существующие. Если у вас есть предложения по улучшению или вопросы по работе бота, я буду рад их обсудить! 