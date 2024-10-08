---
layout: default
title: Быстрый старт
parent: Scout 2.0
grand_parent: AgileX
nav_order: 3
---


# Быстрый старт
## Краткое описание 
Модель представляет собой готовую платформу для различных сценариев применения, имеет широкий спектр возможностей для разработки, адаптации к различным сферам деятельности, например беспилотной доставки внутри помещений. Он имеет мощную моторную систему, способную выдерживать высокие нагрузки. Комбинация двухколесного шасси позволяет ему перемещать грузы весом до 50 кг.

Дополнительные компоненты, такие как стереокамера, лазерный радар, GPS, IMU модуль, манипулятор и компоненты машинного зрения, могут быть установлены пользователем.

## Интерфейсы

### Задняя панель


![Задняя панель](/assets/images/scout_2.0_scheme_rear.png){: width="600px" style="display: block; margin: 0 auto"}


На этой панели располагаются:

|Q1|Тумблер включения|
|Q2|Штырьевой разъем (C14) для заряда аккумулятора|
|Q3|-|
|Q4|Зуммер (звукоизлучатель)|
|Q5|Авиационный разъем для подключения внешнего оборудования 24V + СAN|
|Q6|Индикатор заряда аккумулятора|



![Задняя панель](/assets/images/scout_2.0_rear_panel.png){: width="750px" style="display: block; margin: 0 auto"}


### Передняя панель

![Передняя панель](/assets/images/scout_2.0_front_panel.png){: width="750px" style="display: block; margin: 0 auto"}


### Верхняя панель
Верхняя панель включает в себя 2 разъема:
- CAN+24V (авиационный разъем для подключения внешнего оборудования, дублирующю аналогичный разъем с задней панели)
- RS-232 (разъем DB-9)

![Верхняя панель](/assets/images/scout_2.0_top_panel.png){: width="750px" style="display: block; margin: 0 auto"}


## Начало работы

{: .note }
Убедитесь, что **кнопки экстренной остановки** на краях платформы отжаты.

Для того, чтобы **включить робота**, необходимо повернуть тублер включения питания **Q1** на задней панели, после этого загорится индикатор с уровнем заряда.


Робот готов к работе. 

{: .note }
> Обязательным пунктом на этапе эксплуатации служит предварительный внешний осмотр робота перед каждым включением на наличие дефектов: повреждение проводки, отсутствие защищающих элементов корпуса, раскрученных винтов и прочих моментов, отличающихся от первоначального вида робота (в случае обнаружения дефектов дальнейшая эксплуатация робота возможна, однако мы не сможем гарантировать дальнейшее обслуживание в рамках гарантийного договора).
> 
> Если обнаружен дефект, требуется обратиться к нашим инженерам в службу поддержки через портал [ROBOHELP](https://robohelp.3logic.ru){:target="_blank"}, они смогут оперативно ответить на любые интересующие вопросы.



Для запуска платформы используется тумблер **Q1** на задней панели.
Включите пульт одновременным зажатием обеих кнопок **POWER**. Все переключатели должны быть подняты в верхнее положение.

![Пульт](/assets/images/scout_2.0_remotecontroller.png){: width="600px" style="display: block; margin: 0 auto"}

Далее используйте переключатели SWA, SWB, SWC, SWD:

|SWA|Резерв|
|SWB|Режим управления: верхнее положение - **Command Control Mode**; среднее положение - **Remote Control Mode**; нижнее положение - резерв|
|SWC|Управление светом: верхнее положение - **плавное мерцание**; среднее положение - **постоянное свечение**; нижнее положение - **постоянное свечение при движении**|
|SWD|Резерв|

Используйте переключатель **SWB** чтобы перевести платформу в режим управления с пульта (**Remote Control Mode**). После этого вы можете использовать стики для управления движением.

Верхнее положение переключателя **SWB** потребуется при управлении через CAN (**Command Control Mode**). К платформе прилагается документация с перечнем команд для взаимодействия через CAN. 

По умолчанию пульт не требует каких-либо настроек, однако в случае некорректной работы, воспользуйтесь для его конфигурирования руководством ниже.


## Конфигурирование пульта управления

{: .note }
Пульт управления является универсальными и на нем предварительно настроена привязка, соответствующая используемой модели робота. Не изменяйте привязку в настройках, иначе нормальное управление будет недоступно.

### Настройка используемой модели
  1. Разблокируйте контроллер долгим нажатием на значок замка
  ![Настройка пульта ДУ](/assets/images/rcset.png){: style="display: block; margin: 0 auto"}
  2. Откроется меню **Function**
  3. Выберите _System_
  ![Настройка пульта ДУ](/assets/images/rcset1.png){: style="display: block; margin: 0 auto"}
  4. Нажмите на _Models_
  5. Выберите **“Model 1”** (4.1) и нажмите стрелочку назад (4.2)
  ![Настройка пульта ДУ](/assets/images/rcset2.png){: style="display: block; margin: 0 auto"}
  6. Вернитесь в **Function**	
  7. Выберите **Aux. channels**
  ![Настройка пульта ДУ](/assets/images/rcset3.png){: style="display: block; margin: 0 auto"}
  8. Выберите _Channel 5_
  ![Настройка пульта ДУ](/assets/images/channel5.jpg){: width="500px" style="display: block; margin: 0 auto"}
  
### Настройка канала получения информации

Далее настройте каналы связи следующим образом: _Channel 5 – VRx – Vr A_

Пример настройки Channel 5 – VRx – Vr A:

1. Нажмите на _Значок селектора_:
![Настройка пульта ДУ](/assets/images/rcset5.jpg){: width="100px" style="display: block; margin: 0 auto"}
2. Выберите _VRx_
3. Нажмите на окно _VrA_
![Настройка пульта ДУ](/assets/images/rcset6.png){: style="display: block; margin: 0 auto"}
4. Выберите `VrA` из установки выше, если значение не было установлено по умолчанию:
![Настройка пульта ДУ](/assets/images/rcset7.png){: style="display: block; margin: 0 auto"}
5. Проделайте аналогичные операции с другими каналами связи, значения которых представлены ниже:

```
Channel 6: – SWx – SWC
Channel 7 – SWx – SWA
Channel 8 – SWx – SWB
Channel 9 – SWx – SWD
Channel 10 – KEY – KEY1
```
После этого нажмите на кнопку выхода и перезагрузите контроллер.
  ![Настройка пульта ДУ](/assets/images/rcset8.png){: style="display: block; margin: 0 auto"}
  
### Калибровка контроллера

1. Разблокируйте стартовый экран
2. Выберите вкладку **System** и нажмите на _Stick adjust_
![Настройка пульта ДУ](/assets/images/rcset9.png){: style="display: block; margin: 0 auto"}
3. Далее необходимо левым и правым стиком выполнить следующие действия (последовательность неважна):

```
Левый стик вверх (до упора)
Левый стик вниз (до упора)
Левый стик влево (до упора)
Левый стик вправо (до упора)
Правый стик вверх (до упора)
Правый стик вниз (до упора)
Правый стик влево (до упора)
Правый стик вправо (до упора)
Колеса VRA и VRB влево и вправо до упора
```

Результатом успешной калибровки служит заполненная индикация значений `MR1, MR2, MR3, MR4, VRA, VRB` (допустимы небольшие отклонения, как показано на рисунке):
   ![Настройка пульта ДУ](/assets/images/rcset10.png){: style="display: block; margin: 0 auto"}
   После этого нажмите на кнопку выхода и перезагрузите контроллер
   ![Настройка пульта ДУ](/assets/images/rcset8.png){: style="display: block; margin: 0 auto"}



## Зарядка

1. Убедитесь, что платформа выключена (тумблер питания **Q1** выключен)
2. Вставьте вилку зарядного устройства в разъем **Q2** на задней панели робота.
Индикатором полного заряда служит датчик на блоке питания, который изменит свой цвет с красного на зеленый. Ближе к концу происходит **импульсная зарядка**, вследствие чего из зарядного устройства в течении получаса раздаются щелчки реле, это нормально.

![Блок питания](/assets/images/charging1.png){: style="display: block; margin: 0 auto"}



## FAQ

---

**Q**: Платформа включена, но не реагирует на пульт дистанционного управления. Что делать?

**A**: Сначала проверьте, находится ли аккумулятор в заряженном состоянии, а так же не нажата ли кнопка аварийной остановки. Затем проверьте, выбран ли правильный режим управления с помощью переключателя `SWB`. В последнюю очередь проверьте настройки пульта дистанционного управления.

---

**Q**: Робот начал издавать звуковые сигналы при движении/ожидании, как это исправить?

**A**: Этот звук сигнализирует о низком заряде аккумулятора, необходимо проверить заряд и поставить его на зарядку. Однако это могут быть и внутренние ошибки. Если зарядка не помогла, проверьте соответствующие коды ошибок через шину CAN или обратитесь в службу поддержки через портал [ROBOHELP](https://robohelp.3logic.ru){:target="_blank"}.

--- 

     

