# diploma-experience


## Робот-манипулятор

Целью данной работы было разработать систему управления многозвенным роботом-манипулятором на базе микроконтроллера STM32F7 с использованием ChibiOS.

Основные задачи:
- сборка прототипа манипулятора;
- решение прямой и обратной задач кинематики;
- разработка структуры системы управления; 
- разработка пользовательского интерфейса;
- тестирование реализованной системы управления.

Основные технологии используемые в данной работе:
C/C++ и ChibiOS, Java и Android Studio, Python, OpenCV

Собранный прототип на основе модели https://github.com/4ndreas

<p align="center">
<img src="manipulator_pics/Prototype.png" width="200">
</p>


### Основные компоненты исследуемого робота-манипулятора

<p align="center">
<img src="manipulator_pics/Components.png" width="600">
</p>

### Ручное управление манипулятором


В представленных видео показано разработанное приложение на Java имитирующее управление джойстиком.
Приложение напрямую связывается с управляющим микроконтроллером по Bluetooth соединению. И позволяет управлять манипулятором в двух режимах.
           
<div align="center">
<table>
  <tr>
    <td>
      <figure>
        <figcaption>Управление каждым из двигателей</figcaption>
        <img src="https://github.com/Alionaaaa/diploma-experience/blob/main/manipulator_pics/manual_control_mode_1.gif" alt="Управление каждым двигателем" width="200"/>
      </figure>
    </td>
    <td>
      <figure>
        <figcaption>Управление координатой хвата</figcaption>
        <img src="https://github.com/Alionaaaa/diploma-experience/blob/main/manipulator_pics/manual_control_mode_2.gif" alt="Управление хватом" width="200"/>
      </figure>
    </td>
  </tr>
</table>
</div>


### Структура системы управления


<p align="center">
<img src="manipulator_pics/control_system.png">
</p>



### Алгоритм работы программы

<p align="center">
<img src="manipulator_pics/work_algorithm.png" width="600">
</p>


### Результат работы


В представленных видео наглядно показана работа системы управления, которая позволяет передвигать целевые объекты, строя при этом траекторию с учетом препятствий и обладающая достаточной точностью для передвижения простых объектов.


Пользовательское приложение написанное на Python для детекции и выбора целевых шашек:

<p align="center">
<img src="https://github.com/Alionaaaa/diploma-experience/blob/main/manipulator_pics/detection.gif" width="400">
</p>



<div align="center">
<table>
  <tr>
    <td>
      <figure>
        <figcaption>Построение одной башенки (из выбранных пользователем)</figcaption>
        <img src="https://github.com/Alionaaaa/diploma-experience/blob/main/manipulator_pics/one_tower.gif" alt="Одна башенка" width="200"/>
      </figure>
    </td>
    <td>
      <figure>
        <figcaption>Сортировка шашек по цвету</figcaption>
        <img src="https://github.com/Alionaaaa/diploma-experience/blob/main/manipulator_pics/sort_towers.gif" alt="Две башенки" width="200"/>
      </figure>
    </td>
  </tr>
</table>
</div>

## Гексакоптер

Целью данной работы было разработать базовый функционал по стабилизации гексакоптера на базе микроконтроллера STM32F7 с использованием ChibiOS.

Основные задачи:
- разработка опытного образца шестивинтового БПЛА;
- разработка системы определения ориентации; 
- разработка структуры системы управления;
- тестирование реализованной системы управления

Основные технологии используемые в данной работе:
C и ChibiOS, MATLAB, SolidWorks, Altium Designer

### Основные компоненты исследуемого мультикоптера

<p align="center">
<img src="hexacopter_pics/components.png" width="600">
</p>


### Структура системы управления


<p align="center">
<img src="hexacopter_pics/control_system.png">
</p>


### Алгоритм работы программы:


<p align="center">
<img src="hexacopter_pics/work_algorithm.png" width="600">
</p>


### Результат работы

Ниже представлены графики отработки ПИД-регуляторов

<div align="center">
<table>
  <tr>
    <td>
      <figure>
        <img src="hexacopter_pics/roll.png" alt="Одна башенка" width="200"/>
      </figure>
    </td>
    <td>
      <figure>
        <img src="hexacopter_pics/pitch.png" alt="Две башенки" width="200"/>
      </figure>
    </td>
  </tr>
</table>
</div>

В представленном видео наглядно показана работа системы стабилизации(во избежание чрезвычайно ситуации человек лишь слега придерживает коптер). 
Дальнейшее развитие проекта должно быть направлено в сторону  обеспечения полноценной возможности для тестирования гексакопетра, доработки системы стабилизации и расширения возможностей полётного контроллера


<p align="center">
<img src="https://github.com/Alionaaaa/diploma-experience/blob/main/hexacopter_pics/work.gif" width="400">
</p>
