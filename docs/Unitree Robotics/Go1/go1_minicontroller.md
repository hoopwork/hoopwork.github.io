---
layout: default
title: Использование миниконтроллера
parent: Go1
grand_parent: Unitree Robotics
nav_order: 5
---


# Использование миниконтроллера

## Ручное управление

1. Включите робота и дождитесь пока он проведет инициализацию всех систем и встанет самостоятельно. Кроме того, необходимо дождаться индикации светодиодами на голове. Модуль связи с миниконтроллером находится в голове робота, поэтому он должен также прогрузиться.
2. Включить мини-контроллер одним коротким и одним длинным нажатием на клавишу **POW**
3. Далее можно управлять перемещением робота, используя стик на миниконтроллере (если робот не реагирует на движения стика, пожалуйста подождите еще около 30 секунд и проверьте снова)

## Режим следования за человеком
1. Необходимо надеть миниконтроллер на ремень на его фронтальную часть (сам миниконтроллер должен располагаться перпендикулярно по отношению к боковой части робота (левой его стороны). Пожалуйста, не используйте миниконтроллер, повернувшись к собаке фронтальной стороной корпуса. В противном случае робот начнет пытаться неконтролируемо переместиться к человеку сбоку, что может привести к случайным столкновениям со всеми вытекающими последствиями.

2. Подключитесь к WI-FI робота, используя мобильный телефон и зайдите в
приложение **Unitree Go1** во вкладку `VISION` и проверьте, что соединение
установлено (вы смогли подключиться к камерам робота).

3. Далее откройте `Настройки -> Peripherals -> Track Tag`. В этом окне будут отображаться различные значения с миниконтроллера, динамически изменяющиеся каждую секунду. Это говорит о том, что связь между роботом и микроконтроллером установлена.

4. Для перехода в режим следования, в этом же окне нажмите на кнопку **OFF** напротив строки `FOLLOW`, тем самым вы активируете режим следования в настройках

5. Для того, чтобы робот начал движение в режиме следования, нажмите 2 раза (короткие быстрые нажатия) на кнопку **MOD** на микроконтроллере.

6. После этого робот начнет движение сбоку от вас (если робот не начал движение, переместите его вперед и назад, используя стик на микроконтроллере и вернитесь к п. 5).

7. Для перехода в режим бега, используя режим следования, необходимо также нажать 2 раза на кнопку **MOD** (короткие быстрые нажатия)
