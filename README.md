<!DOCTYPE html>
<html lang="ru">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>First form</title>
    </head>
    <body>
        <header></header>
        <main>
            <form action="" method="post">
                <fieldset>
                    <legend>Основные данные</legend>

                    <label for="username">Имя пользователя</label>
                    <input 
                        type="text"
                        id="username"
                        name="username"
                        placeholder="Введите имя пользователя"
                        minlength="3"
                        maxlength="30"
                        autocomplete="username"
                        required
                    />
                    <hr>

                    <label for="email">Электронная почта</label>
                    <input
                        type="email"
                        id="email"
                        name="email"
                        placeholder="exaple@gmail.com"
                        autocomplete="email"
                        required
                    />
                    <hr>

                    <label for="password">Пароль</label>
                    <input
                        type="password"
                        id="password"
                        name="password"
                        placeholder="Введите пароль"
                        minlength="7"
                        autocomplete="new-password"
                        required
                    />
                    <hr>

                    <label for="phone">Телефон</label>
                    <input
                        type="tel"
                        id="phone"
                        name="phone"
                        pattern="\+?7\d{10}"
                        placeholder="+7 (999) 999-99-99"
                        autocomplete="tel"
                        required
                    />
                    <hr>

                    <label>Возраст</label>
                    <input
                        type="number"
                        id="age"
                        name="age"
                        placeholder="Введите возраст"
                        min="18"
                        max="110"
                    />
                    <hr>

                    <label for="birthdate">Дата рождения</label>
                    <input type="date" id="birthdate" name="birthdate" />
                    <hr>

                    <label for="website">Сайт</label>
                    <input
                        type="url"
                        id="website"
                        name="website"
                        placeholder="https://example.com"
                    />
                    <hr>

                    <label for="search">Поиск</label>
                    <input
                        type="search"
                        id="search"
                        name="search"
                        placeholder="Введите запрос"
                    />
                </fieldset>

                <fieldset>
                    <legend>Дополнительные данные</legend>

                    <label for="mood">Настроение от 1 до 100</label>
                    <input
                        type="range"
                        id="mood"
                        name="mood"
                        min="1"
                        max="100"
                        step="1"
                        value="50"
                    />
                    <hr>

                    <label for="favoriteColor">Любимый цвет</label>
                    <input type="color" id="favoriteColor" name="favoriteColor" value="#ff0000">
                    <hr>

                    <label for="photo">Ваше фото</label>
                    <input type="file" id="photo" name="photo" accept="image/*">
                    <hr>

                    <input type="hidden" name="userId" value="12345">

                    <label id="about">О себе</label>
                    <textarea id="about" name="about" rows="4" cols="50" placeholder="Расскажите о себе">
                    </textarea>
                    <hr>

                    <label>Страна</label>
                    <select id="country" name="country">
                        <option value="" selected>Выберите страну</option>
                        <option value="russia">Россия</option>
                        <option value="usa">США</option>
                        <option value="germany">Германия</option>
                        <option value="france">Франция</option>
                    </select>
                </fieldset>

                <fieldset>
                    <legend>Любимые овощи</legend>
                    <label><input type="radio" name="veg" value="cucumber">Огурец</label>
                    <label><input type="radio" name="veg" value="tomato">Помидор</label>
                    <label><input type="radio" name="veg" value="potato">Картошка</label>
                </fieldset>

                <fieldset>
                    <legend>Согласия</legend>
                    <label for="policy">Согласен с политикой</label>
                    <input type="checkbox" id="policy" name="policy" required>
                    <label for="terms">Согласен с условиями</label>
                    <input type="checkbox" id="terms" name="terms" required>
                </fieldset>

                <button type="submit">Отправить</button>
                <button type="reset">Сбросить</button>
            </form>
        </main>
        <footer></footer>
    </body>
