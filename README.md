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
C/C++, Java и Android Studio, Python, OpenCV

Собранный прототип на основе модели https://github.com/4ndreas

<p align="center">
<img src="manipulator_pics/Prototype.png width="200"">
</p>


### Основные компоненты исследуемого робота-манипулятора

Основными компонентами являлись:

<p align="center">
<img src="manipulator_pics/Components.png">
</p>

### Ручное управление манипулятором


В представленных видео показано разработанное приложение на Java имитирующее управление джойстиком.
Приложение напрямую связывается с управляющим микроконтроллером по Bluetooth соединению. И позволяет управлять манипулятором в двух режимах.

Управление каждым из двигателей                                    Управление координатой хвата              
<div align=center>
<table>
  <tr>
     <td><img src="https://github.com/Alionaaaa/diploma-experience/blob/main/manipulator_pics/manual_control_mode_1.gif" alt="dfs" width="200"/></td>
    <td><img src="https://github.com/Alionaaaa/diploma-experience/blob/main/manipulator_pics/manual_control_mode_2.gif" alt="dfs" width="200"/></td>
  </tr>
</table>
</div>


### Структура системы управления


<p align="center">
<img src="manipulator_pics/control_system.png">
</p>


Алгоритм работы программы:

<p align="center">
<img src="manipulator_pics/work_algorithm.png">
</p>


### Результат работы


В представленных видео наглядно показана работа системы управления, которая позволяет передвигать целевые объекты, строя при этом траекторию с учетом препятствий и обладающая достаточной точностью для передвижения простых объектов.


Пользовательское приложение написанное на Python для детекции и выбора целевых шашек:

<p align="center">
<img src="detection.gif">
</p>

  

<p align="center">
<img src="one_tower.gif">
</p>





Построение одной башенки из выбранных пользователем шашек:                                    Сортировка шашек по цвету:             
<div align=center>
<table>
  <tr>
     <td><img src="https://github.com/Alionaaaa/diploma-experience/blob/main/manipulator_pics/one_tower.gif" alt="dfs" width="200"/></td>
    <td><img src="https://github.com/Alionaaaa/diploma-experience/blob/main/manipulator_pics/sort_towers.gif" alt="dfs" width="200"/></td>
  </tr>
</table>
</div>
