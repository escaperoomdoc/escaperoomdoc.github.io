# Наименование и обозначение комнат, изделий, декора и кабелей

## Комнаты

Комнаты обозначаются большими латинскими буквами. Всем стенами присваиваются номера,
что позволяет обозначить каждую плоскость стены в каждой комнате.
Например, плоскость левой стены комнаты _**А**_ будет обозначаться _**A1**_, правой - _**A6**_,
верхней - _**A2**_, нижней —  _**A5**_.

![proj-room](../assets/layout/proj-room.png ':size=600')

## Изделия

Каждое изделие обозначается арабскими числами. Нумерация изделий сквозная.

Изделия подразделяются на следующие группы:
 - _**декор**_ — изделия, служащие для украшения. Кабели к данными элементам не подводятся, игроки с ними не взаимодействуют;
 - _**игровые элементы**_:
   - _**автономные**_ — изделия, непосредственно участвующие в игре, но не имеющие электрических элементов. Подведение кабелей к данными изделиями не предусмотрено;
   - _**электрические**_ — изделия, имеющие в своём составе электрические объекты. Количество и типы подводимых кабелей определяются устройством изделия;
 - **свет** - изделия, служащие для освещения.

Для изделий предусмотрены следующие условные обозначения:

|          Тип изделия          |                     Обозначение                      |
|:-----------------------------:|:----------------------------------------------------:|
|             декор             |   ![](../assets/layout/proj-decor.png ':no-zoom')    |
|  автономный игровой элемент   | ![](../assets/layout/proj-autonomous.png ':no-zoom') |
| электрический игровой элемент |  ![](../assets/layout/proj-electric.png ':no-zoom')  |
|             свет              |   ![](../assets/layout/proj-light.png ':no-zoom')    |

!> **Нужно подумать, нужно ли включать в число изделий камеры и динамики, а также распространять на них сквозную нумерацию.**

## Камеры

Камеры на плане обозначаются арабскими числом и значком камеры. Кабели к камерам имеют наименования вида _**CAM1**_. 
Число в наименовании кабеля должно совпадать с числом для обозначения камеры на плане.

## Динамики

Динамики на плане обозначаются арабскими числом и значком динамика. Кабели к динамикам имеют наименования вида _**SPK1**_.
Число в наименовании кабеля должно совпадать с числом для обозначения динамика на плане.

## Кабели к изделиям

Обозначения кабелей к изделиям составляются из большой латинской буквы и числа, соответствующего изделию.
Используемые для обозначения кабелей буквы приведены в таблице:

| Обозначение кабеля |                                                                 Описание                                                                  |
|:------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------:|
|         S          | Сенсорный провод. Для подключения различных датчиков и слаботочных устройств. Как правило, в качестве сенсорного используется UTP-кабель. |
|         L          |                                                       Кабель к источнику освещения.                                                       |
|         M          |                                                          Кабель к электрозамку.                                                           |
|         R          |                                     UTP-кабель, используемый для передачи данных по стандарту rs485.                                      |
|         D          |                                              Кабель для подключению к изделию питания DC12V.                                              |
|         P          |                                             Кабель для подключения к изделию питания АС220V.                                              |
|         E          |                                                     Кабель для подключения ethernet.                                                      |
|         X          |                                                              Прочие кабели.                                                               |


Например, кабели к изделию _**1**_ будут иметь наименования _**L1**_, _**M1**_, _**S1**_.
Если в составе изделия несколько кабелей одного типа, то наименования будут следующие: _**M1.1**_, _**M1.2**_, _**M1.3**_ и т. д.
Как правило, кабели идут от системы управления к изделиям. В случае, если кабель идёт от одного изделия к другому,
то наименование кабеля будет содержать номера обоих изделий. Например, кабель идущий от изделия _**1**_ к изделию _**2**_ будет иметь наименование _**R1-2**_.

Обозначение кабелей на плане заключается в овал. Высота вывода кабеля обозначается следующим образом: 

- _**h1500**_ - вывод расположен на заданной высоте над уровнем пола, в данном случае на высоте 1500 мм;
- _**floor**_ - вывод на уровне пола;
- _**ceiling**_ - вывод на уровне потолка.




