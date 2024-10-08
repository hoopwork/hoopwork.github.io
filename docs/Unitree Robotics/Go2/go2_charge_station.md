---
layout: default
title: Зарядная станция
parent: Go2
grand_parent: Unitree Robotics
nav_order: 3
---


# Зарядная станция

> С весны 2024 года, зарядка робота с помощью зарядной станции поддерживается **на всех** модификациях.


# Общая информация

Зарядная станция представляет собой напольную пластину с двумя площадками-электродами. Помимо нее, в комплекте имеются 2 металические рамы для сборки вертикальной стойки. Стойка используется для нанесения графических меток, необходимых для машинного зрения и служащими опорой при позиционировании робота. Тип метки произволен, предполагается, что разработчик автономного движения наклеит собственную метку, использующуюся в его системе распознавания.

Контакт робота с зарядной станцией осуществляется через его **2 пары винтов**, расположенных снизу (в передней и задней частях корпуса). 


# Начало работы

> Для удобства описания расположения элементов зарядной станции введем условную точку отсчета, служащей для ориентации в пространстве - надпись **Unitree**.
> 
> Таким образом, если смотреть сверху:
> 
> - **верхняя часть** станции - **над** надписью Unitree.
> 
> - **нижняя часть** станции - **под** надписью Unitree.

Соберите стойку, соединив комплектными винтами две металические рамы, и прикрепите ее к верхней части зарядной станции.

Подключите зарядную станцию к электрической сети с помощью комплектного блока питания. Для плотного прилегания к полу, пропустите сетевой кабель через специальный канал в задней части зарядной станции.

![go2_charge_station](/assets/images/go2_charge_station_1.png){: width="500px" style="display: block; margin: 0 auto"}


Индикатором наличия питания станет мигание светодиодов зеленым светом (2 раза) в боковых частях (слева и справа). После чего характер свечения станет постоянно зеленым, но менее ярким.

При включении зарядной станции в розетку напряжение на электродах **отсутствует** (это можно проверить тестером).


> Сверху располагается - **положительный** электрод.
> 
> Снизу располагается - **отрицательный** электрод.



# Ручная постановка на зарядку

Подведите робота лицом к верхней части зарядной станции. Переведите робота в положение лежа, расслабьте моторы. Робот должен лечь таким образом, чтобы его контакты сомкнулись с электродами станции.

![go2_charge_station](/assets/images/go2_charge_station_2.png){: width="500px" style="display: block; margin: 0 auto"}

Далее между робот и зарядной станцией должна произойти синхронизация. Для этого в голове робота и верхней части станции (ближе к стойке) расположены датчики. Производитель не сообщает какая именно беспроводная технология используется для обмена данными между роботом и станцией, но известно, что дистанция срабатывания очень маленькая, менее 3 см.

После успешной синхронизации робот подаст напряжение на электроды - **32~33** Вольта. Робот начнет заряжаться. Зеленые светодиоды начнут плавно мигать, так же как при включении станции. На аккумуляторе также появится индикация процесса заряда, повторяющую индикацию при заряде от обычного блока питания.

Тот факт, что между роботом и зарядной станцией должна предварительно произойти синхронизация, позволяет сразу ответить на логичные вопросы:

- если на зарядную станцию положить выключенного робота, процесса заряда не будет (из-за отсутствия синхронизации). Заряд будет осуществляться только если **робот включен**.

- зарядная станция подаст напряжение на электроды только при нахождении робота рядом и в правильном положении (лежа, лицом к верхней части станции).

- если собака ляжет наоборот (лицом к нижней части станции), синхронизация не случится и напряжение на контакты не подастся. В любом случае, лишний раз так делать не стоит.



# Автономная постановка на зарядку

> На текущий момент (сентябрь 2024) функционал автоматической постановки робота на зарядку еще находится в разработке у производителя.

Фирменное программное обеспечение с элементами SLAM-функционала для самостоятельной постановки на зарядку робота с помощью распознавания QR-кода на данный момент находится у производителя в разработке. Можно использовать свои метки и распознавать их собственным навигационным ПО.

Вся реализация постановки на зарядку будет настраиваться через мобильное приложение.


---

Upd by Igor P. 04.09.2024
{: .label .label-green }




