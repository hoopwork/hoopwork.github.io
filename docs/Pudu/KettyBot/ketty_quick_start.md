---
layout: default
title: Быстрый старт
parent: KettyBot
grand_parent: Pudu
nav_order: 1
---

# Быстрый старт

Для успешной работы с продуктами **PUDUTech** необходимо установить мобильное приложение на свой смартфон, для этого отсканируйте QR-код с соответсвующим устройством.

!['PuduQRIOS' , 'IOS'}](/assets/images/PuduQR_app_ios.png "ios"){: width="150px" height="150px" style="display: block; margin: 20px auto"}
<center>IOS</center>
![PuduQRAndroid {caption=Android}](/assets/images/PuduQR_app_android.png "Android"){:.image  width="150px" height="150px" style="display: block; margin: 20px auto"}
<center>Android</center>

Или воспользуйтесь прямой ссылкой на [Приложение для IOS](https://apps.apple.com/app/id1598340894) и [Приложение для Андроид](https://business-hongkong-apk.oss-cn-hongkong.aliyuncs.com/apk/prod/PuduLink.apk).


Данное **приложение** обеспечивает удаленный доступ к управлению и менеджменту робота, а так же позволяет получить **Авторизационный код** для безопастного доступа к роботу и его функциям.
Например для любых манипуляций с картами, робот будет запрашивать данный код, либо отсканировать предоставленный QR используя мобильное приложение.

![PuduAuthCode](/assets/images/Pudu_AuthCode.png){:.image style="display: block; margin: 20px auto"}\
**Авторизационный код** можно найти в Центре данных облака **PUDU Cloud** по следующему пути [Store Managment] -> [Store] -> [Details].

![PuduStoreMngmt](/assets/images/Pudu_storemenagment.png){:.image style="display: block; margin: 20px auto"}
![PuduStore](/assets/images/Pudu_StoreDetails.png){:.image style="display: block; margin: 20px auto"}


## Требования к окружению

- Требования к дорожному покрытию

	* Плоскостность: ровность дороги =< 5 мм
	* Уклон: =<5° в противном случае высока вероятность пролить жидкости на подносах
	* Ширина: минимальная ширина прохода для робота составляет 55 см, однако наилучший вариант будет если от робот до стен будет > 80 см с каждой стороны
	* Материал покрытия: пластик, металлические пластины, прорезиненное покрытие, терраццо, ковролин с высотой ворса =< 1 см

![Требования к дороге](/assets/images/Pudu_floor_req.png){: width="900px" height="250px" style="display: block"}

{: .note}
**Покрытие не должно быть мокрым**

- Требования к рабочей зоне

	* Рабочая зона: не должна быть пустой зоной, тоесть должна иметь какие либо препятсвия для автоматического позиционирования и навигации
	* Особые зоны: зоны с большой вероятностью падения или повреждения робота должны быть отмечены на карте робота как опасные, такие как то: рядом с лифтом, рядом с лестницами, рядом с рампами с крутым уклоном, рядом с элеваторами.

- Требования к пути

	* В режиме лазерного лидарного сканирования робот может пропустить **тонкие препятсвия** (диаметром менее 20 мм), тонкие ножки стульев, столов, их необходимо отметить как показано на рисунке ниже.
![]()
	* Если есть черные или зеркальные поверхности и покрытия их необходимо отметить контрастной полосой на высоте 16 см от пола.
![Требования к дороге](/assets/images/Pudu_env_req.png){: width="700px" height="250px" style="display: block"}

## Первоначальная настройка робота

### Первый запуск

Для **первого старта робота в новом месте**, у робота имеется функция создания карт без использования Инструментов маппинга.
1. Начинать работу стоит с выбора и разметки начальной точки для робота. Это могут быть **настенные маркера**
		![KettyWall](/assets/images/Ketty_wall.png){:.image style="display: block; margin: 20px auto"}
 	и **потолочные метки** (поставляются в комплекте с роботом).\
		![KettyFloor](/assets/images/Ketty_floor.png){:.image style="display: block; margin: 20px auto"}
	Их следует разместить в желаемом месте в соотвествии изображениями выше, при этом не стоит их размещать на отражающих 		поверхностях, таких как стекло, керамическая плитка или глянцевые потолки.
2. Установите робота в его начальное положение:\
		- так что бы камера сверху робота смотрела **ровно на потолочные метки**
	![KettyStartPosFloor](/assets/images/Ketty_StartPos_Floor.png){:.image style="display: block; margin: 20px auto"}
		- на растоянии около ~1 метра, так что бы камера спереди робота смотрела **на настенные маркера**
	![KettyStartPosWall](/assets/images/Ketty_StartPos_Wall.png){:.image style="display: block; margin: 20px auto"}
3. Для запуска робота убедитесь, что **ключ вставлен** в разъем слева снизу и **переведен в состояние включения**
	![KettyKeyOn](/assets/images/Ketty_Key.png){:.image style="display: block; margin: 20px auto"}

{: .note}
Пожалуйста не теряйте ключ от робота, он находится в зип-пакете с сертификатом робота.

4. Включение осуществляется коротким удержанием кнопки(около 1 секунды) сверху экрана робота.\
		Выключение удержанием этой кнопки в течении 3 секунд.\
		Касание экрана во время движения поставит робота на паузу, до следующего касания экрана.

### Режим лазерного лидара

1. Запускаем инструмент для маппинга в настройках в приложении на экране робота \
		![KettyApp](/assets/images/Ketty_AppSettings.png){:.image style="display: block; margin: 20px auto"}
2. Выбираем **"Редактирование карт"**\
		![KettyMapEdit](/assets/images/Ketty_mapedit.png){:.image style="display: block; margin: 20px auto"}
3. Создаем новую карту **"New map"**\
		![KettyNewMap](/assets/images/Ketty_newmap.png){:.image style="display: block; margin: 20px auto"}
4. Отмечаем начальную точку и начинаем толкать робота. Сопровождаем его по пути для отстройки всей карты.\
		![KettyMapStart](/assets/images/Ketty_carrymapping.png){:.image style="display: block; margin: 20px auto"}

{: .note}
**Старайтесь не перекрывать камеры робота во время работы.**


![KettyLidarMap](/assets/images/Ketty_lidarmapping.png){:.image style="display: block; margin: 20px auto"}
В завершение сканирования рабочей области нажмите кнопку **"Finish Mapping"**.
5. Выбираем желаемые функции робота (их можно изменить в любое время).
		![KettyFunc](/assets/images/Ketty_function.png){:.image style="display: block; margin: 20px auto"}
6. Модифицируем карту добавляя на нее необходимые объекты взаимодействия и опасные зоны.\
		![KettySpecial](/assets/images/Ketty_app_specialelements.png){:.image style="display: block; margin: 20px auto"}
7. Разграничивайте зоны, в которые робот не должен заезжать виртуальными стенами.\
		![vwall](/assets/images/Ketty_vwall.png){:.image style="display: block; margin: 20px auto"}
8. Для проверки корректности работы верните робота на начальную точку и запустите проезд к любой выбранной точке на карте.

## Добавление промоматериалов

* **Настройка бизнес рекламы**\
	Добавление промоматериалов доступно из облака PUDU Cloud. В том числе с проигрыванием звуковых файлов.\
	![KettyAdvert](/assets/images/Ketty_promoscreen.png){:.image style="display: block; margin: 20px auto"}
	1. Зарегестрировать аккаунт пользователя в облаке и выбрать необходимово робота\
	![KettyAdSelect](/assets/images/Ketty_ad.png){:.image style="display: block; margin: 20px auto"}
	2. Можно либо выбрать уже загруженные ранее рекламные материалы, либо добавить новые, для этого перейдите **"Add Ad"**\
	![KettyAddAd](/assets/images/Ketty_advertising.png){:.image style="display: block; margin: 20px auto"}
	3. В открывшемся окне необходимо выбрать материал, дать ему системное имя, скорректировать длительность, а так же указать период повторяемости.\
	![KettyAdSetting](/assets/images/Ketty_ad_setting.png){:.image style="display: block; margin: 20px auto"}
	4. Вызвать рекламу можно так же через это облако, можно установить последовательность показа перетаскивая рекламные материалы вверх списка.

{: .highlight}
Учтите, загрузить можно изображения в формате **.jpg**, **.jpeg**, **.png** и **.gif** с максимальным весом не более 20Mb. Рекомендуемое разрешение изображения 1080х640 пикселей.\
Видеофайлы должны быть в формате **.mp4**, а их вес не должен превышать 500Mb. Рекомендуемое разрешение трансляции 1080p.
