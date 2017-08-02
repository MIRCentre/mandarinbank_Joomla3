**protocol** - Протокол по которому пользователи заходят на ваш сайт(http или https)

**domain** - Домен вашего сайта

**port** - Порт вашего сайта, если ваш сайт находится на 80 порте, т.е. в адрессной строке после домена через двоеточие не указано число, то данный параметры указывать не прийдётся!

**protocol://domain:port/** - Может быть как `https://example.com/` так и `https://example.com:80/`

## Установка

1. Распаковываем содержимое репозитория в корень сайта
2. Переходим по адрессу **protocol://domain:port/installMandarin.php**  %domain%/installMandarin.php
3. Удаляем **install-mandarin.php** из папки, в которую вы распаковали репозиторий
4. Авторизуемся в панели управления **protocol://domain:port/administrator/**
5. Переходим в `Components` > `Joomshoping` > `Options` > `Payments`
6. Находим и кликаем на `MandarinBank`
7. Нажимаем на вкладку `Config`
8. Заполняем `Merchant ID` и `Merchant Secret`
9. Нажимаем `Save & Close`
10. В системе MandarinPay указываем
- callbackURL **protocol://domain:port/payment-mandarin.php**
- returnURL **protocol://domain:port/result-mandarin.php**
