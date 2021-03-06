## Как войти в админку 101hit.ru

- Перейти на http://101hit.ru/admin/
- Ввести креды для входа: `Пароль: [***]` `Логин: [***]`

## Как отключить клиента от CMS
Шаги по отключению клиента можно пропустить, если этого не требуется и можно перейти сразу к шагу создания заглушки
- Чтобы отключить клиента нужно перейти во вкладку `Спутник`
- Найти сайт, который необходимо отключить
![img.png](screenshots/img.png)
  
- Далее смотрим кто владелец сайта, это можно сделать в колонке `owner`
![img_1.png](screenshots/img_1.png)
  
- Затем переходим во вкладку `Users` и ищем владельца
![img_2.png](screenshots/img_2.png)
  
- Кликаем на Username в нашем случае это `anpe`
- После этого мы попадаем в настройки юзера и перелистываем их в самый низ и находим кнопку `удалить` 
![img_3.png](screenshots/img_3.png)
  
### Заглушка для сайта
  
- Далее сделаем заглушку для сайта, к которому у клиента больше нет доступа
  (Верхние шаги можно не делать, чтобы сохранить запись клиента на случай, если клиент передумает)
  
- Заходим по `ssh` на сервер, креды для входа можно попросить у Виктора Сазонова. Чтобы войти по ssh,
необходимо открыть терминал(macOS/linux)/командную консоль(windows) и набрать:`ssh имяпользователя@ip-адрес сервера`,
  далее потребуется ввести пароль
  
- Далее вбиваем команду в терминал
![img.png](screenshots/img_25.png)
  
- Далее вбиваем команду
![img_3.png](screenshots/img_28.png)
  
- Далее вбиваем команду `ls` в терминал и можем увидеть все конфиги всех сайтов
![img_4.png](screenshots/img_29.png)
  
- Выбираем нужный кофиг(я для примера возьму конфиг сайта anpe.101hit.ru)
и вбиваем команду `nano имяконфига(адрес сайта)`, и должно появится окно с параметрами, которые можно редактировать
  
![img_6.png](screenshots/img_31.png)

- Далее находим строчку, красным выделено имя сайта
![img_7.png](screenshots/img_32.png)
  
- Комментируем строчку(`#` - это значит строка закомментирована) и заменяем ее, то есть все должно выглядеть вот так:
![img_8.png](screenshots/img_33.png)
  
- Находим и комментируем еще одну строчку и заменяем ее, то есть все должно выглядеть вот так:
![img_9.png](screenshots/img_34.png)
  
- Далее нажимаем `ctrl+x` и появляется окно
![img_10.png](screenshots/img_35.png)
  Нажимаем `y` и нажимаем `enter`
  
- Далее пишем в терминале и нажимаем `enter`:
![img_13.png](screenshots/img_38.png)
  
- Теперь при входе на сайт будет:
![img_14.png](screenshots/img_39.png)
  
### Как разблокировать сайт

- Чтобы разблокировать сайт вам необходимо: проделать все шаги, которые gпоказаны на скриншоте,
только нужно закомментировать строчки, где есть красный эллипс и раскоментировать строчки, где его нет
  
![img.png](screenshots/img_40.png)

## В меню Geo objects

![img_4.png](screenshots/img_14.png)

- Находятся объекты, которые отображаются на карте
  Это меню не нужно трогать, тк скорее всего это отображение объектов из БД


## В меню Satellite
![img_4.png](screenshots/img_4.png)

- Во вкладке `Спутник` можно добавить сайт и добавить описания для него, а также указать Yandex verification meta и Google verification meta

![img_5.png](screenshots/img_5.png)

- На вкладке `Страницы спутников` находится заголовки страниц с содержимым

![img_6.png](screenshots/img_6.png)

- В фильтре можно выбрать конкретный сайт и просмотреть все заголовки с содержанием, которое принадлежит выбранному сайту

![img_7.png](screenshots/img_7.png)


## В меню Shop

- В меню `Shop` различные настройки типов и групп товаров которые будут отражаться в личном кабинете у владельца `сайта(Спутника)`

## В меню Contractor

![img_8.png](screenshots/img_8.png)

- В этих вкладках содержится информация о `контрагентах` которые можно выбрать при создании `спутника`, а также информацию о банках и клиентах, то есть записях, под которыми входят владельцы `сайтов`

![img_9.png](screenshots/img_9.png)

- Профиль можно активировать или деактивировать 

## Аккаунт клиента

- В аккаунте клиента можно редактировать содержимое страниц сайта, а также добавлять новые страницы 

### Вход в аккаунт клиента

- Заходим на http://101hit.ru/ `Перед тем как перейти на 101hit, нужно выполнить вход как администратор`

![img.png](screenshots/enter.png)

- Далее вводим владельца сайта `(owner)` в строку `Войти как`

![img_10.png](screenshots/img_10.png)

- В меню `Контрагенты` можно выбрать контрагента и изменить контактную информацию

![img_1.png](screenshots/img_11.png)

- В меню `Группы товаров` можно редактировать описание товара, а также менять картинки сопутствующие данному товару (В секции `Доп.группы товаров` возможно тоже самое но в)

![img_2.png](screenshots/img_12.png)

- На сайте http://alfa.live/ товары находятся в разделе услуги, на других сайтах эта секция может называться по другому, например `каталог`

![img_3.png](screenshots/img_13.png)

- При нажатии на товар в нашем случае `Строительство бассейнов` в разделе группы товаров, откроется редактирование информации о товаре, которая отражена на сайте

![img.png](screenshots/img_16.png)

- На сайте альфы есть список поставщиков/производителей

![img_1.png](screenshots/img_17.png)


- Чтобы его изменить необходимо перейти в меню `Производители`, там будет список из всех производителей, в который можно добавить нового производителя или изменить название или картинку о старом производителе

![img_2.png](screenshots/img_18.png)

- В меню `Фотогалереи` можно создать галереи, которые будут отражаться на страницах сайтов

![img_3.png](screenshots/img_19.png)

- Ниже представлен пример, где можно использовать фотогалереи.
Фото галерею можно добавить на страницу сайта в настройках `Страницы сайта`

![img_4.png](screenshots/img_20.png)

- В меню `Баннеры` можно добавить баннеры, которые будут отображаться на сайте или изменить существующие 

![img_5.png](screenshots/img_21.png)
Ниже представлен пример, где баннеры отображены на сайте

![img_6.png](screenshots/img_22.png)

### Меню Страницы сайта

![img_7.png](screenshots/img_23.png)

- В меню `Страницы сайта` можно редактировать содержимое отображаемых страниц на сайте или создавать новые страницы.
Ниже представлены все страницы сайта альфы, содержимое которых можно редактировать
  ![img_9.png](screenshots/img_24.png)
  



