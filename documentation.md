# ZONBIROVANIE - Документация

**Описание проекта**

ZONBIROVANIE — это веб-приложение, которое используется для определения нефтяных загрязнений на поверхности морей РФ (Чёрное и Азовское) по данным снимков ДЗЗ.

**Структура проекта**

Проект организован следующим образом:
```
/zonbirovanie
│── /frontend                           # Каталог с фронтендом
│   │── /scr                            # Папка с html/css компонентами проекта
│   │   ├── /css                        # Папка с css
│   │   │   ├── style.css               # css для главной страницы
│   │   │   ├── styleloading.css        # css для страницы загрузки изображений
│   │   │   ├── stylelogin.css          # css для страниц входа и регистрации
│   │   ├── /images                     # Папка с изображениями
│   │   │   ├── asia.svg                
│   │   │   ├── circle.svg           
│   │   │   ├── ellipse.png    
│   │   │   ├── loading-cloud.svg                
│   │   │   ├── logo-log-in.svg
│   │   │   ├── logo.svg
│   │   │   ├── rectangle.png
│   │   │   ├── user-icon.svg
│   │   │   ├── wave-loading.svg
│   │   │   ├── wave-log-in.svg
│   │   │   ├── wave.svg
│   │   ├── index.html                 # Главная страница
│   │   ├── loading.html               # Страница для загрузки изображений
│   │   ├── login.html                 # Страница с входом
│   │   ├── signup.html                # Страница с регистрацией
│   │── README.md
```
🎨 Основные компоненты
1. Форма входа (index.html)
Форма входа содержит:

Поле для ввода почты
Поле для ввода пароля
Сообщение об ошибке (появляется при неверном вводе)
Кнопку "Продолжить" для отправки формы
Ссылку на регистрацию
Ключевая разметка:

html
Копировать
Редактировать
<form action="">
    <h1>Вход в аккаунт</h1>
    <div class="divider"></div>

    <div class="input-box">
        <label for="email">Почта</label>
        <input type="email" id="email" required>
    </div>

    <div class="input-box">
        <label for="password">Пароль</label>
        <input type="password" id="password" required>
        <span class="error-message">Неверно введена почта или пароль</span>
    </div>

    <button type="submit" class="btn">Продолжить</button>
</form>
2. Визуальные стили (log_in_style.css)
Файл log_in_style.css отвечает за стилизацию страницы, включая:

Цветовую палитру
Отступы
Размещение элементов
Шрифты
Ключевые моменты стилизации:

css
Копировать
Редактировать
body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: #060935;
}

.wrapper {
    width: 90%;
    max-width: 420px;
    background: #fff;
    border-radius: 30px;
    padding: 30px 40px;
}
3. Подключенные шрифты
Шрифты загружаются через @import:

css
Копировать
Редактировать
@import url('https://db.onlinewebfonts.com/c/75e6e29986cbf78e3aaebb7c39b0eac3?family=IntroFriday');
@import url('https://fonts.googleapis.com/css2?family=Alike+Angular&family=Montserrat:wght@100..900&display=swap');

**Запуск сервера frontend**

1. Из корня проекта перейдите в папку frontend:

    cd frontend

2. Установите зависимости:

    npm install

3. Запустите сервер:

    npm run dev

**Контакты**

Если у вас есть вопросы, обращайтесь:
tg: @vlad6268