Плагин авторизации и интеграции с соцсетями для AltoCMS
=======================================================

Использованы иконки ХабраПака (https://github.com/Incwadra/HabraPack)
Наименования файлов изменены в соответствии с требованиями плагина.

##1. Установка
Устанавливается как обычный плагин, но для того, что бы заработала связь с социальными сетями,
для каждой нужно создать приложение и получить идентификатор приложения и секретный ключ, которые
нужно указать в админке плагина в разделе «Контент». Из файлов конфига ничего не берется,
поэтому писать туда ничего не нужно.


Порядок создания приложения и получения ключей для разных социальных сетей следующий:

###1.1. ВК
По адресу: https://vk.com/dev справа вверху нажимаем кнопку «создать приложение» и создаем
приложение типа «Standalone-приложение». Затем на страничке «Настройки» этого приложения
получаем ID приложения и Защищенный ключ, которые пишем в настройки плагина.

###1.2. Одноклассники
Нужно получить права разработчика здесь - http://www.odnoklassniki.ru/devaccess
После получения этих прав вам предложет перейти по ссылке на страницу ваших приложений,
где нужно создать новое приложение типа «Внешнее приложение». Ему можно присвоить
статус «Скрытое», поскольку переходить в него будут по ссылке. Все ключи придут вам на почту.

###1.3. Фейсбук
Создаем новое приложение здесь - https://developers.facebook.com/apps
На страничке «Status & Review» делаем его публичным. Берем ключи и подставляем в настройки плагина.

###1.4. Твитер
Приложение создается здесь - https://dev.twitter.com/apps/new
Нужно ему указать права на публикацию от имени пользователя, но для этого нужно к Твитеру
привязать телефон и отправить в качестве подтверждения СМС-ку с него, а она платная, цену не
помню, но кажется по цене оператора.
Все ключи там же, на странице создания приложения. В свойство «Callback URL» нужно
записать «http://ВАШСАЙТ /auth/tw»

###1.5. Мой Мир
Приложение создается здесь - http://api.mail.ru/sites/my/add
Ключи в настройках приложения

###1.6. Яндекс
Приложение создавать нужно здесь - https://oauth.yandex.ru/client/new
В нем выбрать в пункте «Яндекс.Логин» Все права, то есть Адрес, дату рождения, Имя и пол.
Ключи в приложении, В свойство «Callback URI» нужно записать «http://ВАШСАЙТ /auth/ya»

###1.7. Google
Приложение создавать нужно здесь - https://code.google.com/apis/console#access
В свойство «REDIRECT URIS» нужно записать «http://ВАШСАЙТ /auth/g»


###1.8. GitHub
На странице https://github.com/settings/applications создаем новое приложение
кнопкой «Register new application»
В свойство «Authorization callback URL» нужно записать «http://ВАШСАЙТ /auth/ github»


###1.9. Инстаграм
Здесь – http://instagram.com/developer/clients/register/ создаем новое приложение
В свойство «Authorization callback URL» пишем «http://ВАШСАЙТ /auth/i»


###1.10. LinkenId
Здесь – https://www.linkedin.com/secure/developer добавляем новое приложение
Устанавиваем ему право «r_basicprofile», затем В свойство «URL-адреса переадресации OAuth 2.0:»
пишем «http://ВАШСАЙТ /auth/li»

