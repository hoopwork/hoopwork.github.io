---
layout: default
title: Снятие логов
parent: AlienGo
grand_parent: Unitree Robotics
nav_order: 4
---


# Снятие логов

Основная плата управления в реальном времени постоянно отправляет поток отладочных данных, которые используются для диагностики. На спине робота AlienGo располагаются два диагностических разъема (RS-485). Подключаемся к тому из них, который расположен левее (если голова собаки располагается сверху):

![Пример подключения для снятия логов](/assets/images/AlienGoLogPlugIn.jpg){: width="500px" style="display: block; margin: 0 auto"}

Устройство (робособака) должно определиться как COM-порт. Любым терминалом (например **putty**) слушаем этот COM-порт.


```
Скорость: 115200
Формат кадра: 8-N-1
```
	
Пример вывода:

![Пример вывода логов](/assets/images/logExample.jpg){: width="600px" style="display: block; margin: 0 auto"}




