# Оценка параметров кабелей

## Теория

Кому не интересна теория, можно пропустить этот раздел сразу перейти к выводам. Кому интересно, читаем...
Большая часть питания квеста мы рекомендуем 12V, как это безопасное напряжение и дальнейшие расчеты будут отталкиваться именно от этого номинала (для других номиналов подход в принципе похожий).
Считаем, что до устройства должно дойти не менее 5% от 12V, т.е. около 11.5V, то есть максимальное падение dU на кабеле может быть не более 12V-11.5V=0.5V (это наш критерий).
Предположим, что мощность конечного устройства (нагрузки типа ленты или замка) составляет «Pmax» Ватт. Тогда ток через устройство по 12V будет равен Imax=Pmax/12.
Если в паспорте устройства указан максимальный ток Imax, то можно использовать его в качестве основы для будущих вычислений.  

Итак, имеем: максимальное допустимое падение на кабеле dU=0.5V, максимальный ток Imax берем с паспорта или вычисляем по формуле Imax=Pmax/12. По закону Ома максимальное сопротивление кабеля должно быть R = dU / Imax = 0.5 / Imax. С другой стороны, сопротивление кабеля равно R = 2 * p * L / S, где p – удельное сопротивление (для меди всегда равно 0.018), L – длина трассы кабеля, S – площадь сечения кабеля в мм2 – искомая величина, и умножаем на 2, так ток проходит до устройства и обратно по кабелю. Итак получаем:  
0.5/Imax = R = 0.036 * L / S, откуда находим:  
S = 0.072 * L * Imax, где L – длина трассы, I – максимальный ток или учитывая, что Imax = Pmax / 12,  
S = 0.006 * L * Pmax, где L – длина трассы, P – максимальная мощность.  

## Примеры 

**P1**. Пример расчета для 15 метров LED-ленты, которая находится на расстоянии 5 метров от источника питания. Допустим мощность 14.4 Вт/метр, тогда 15 метров потребит 216Вт. Минимальное сечение кабеля будет составлять S = 0.006 * 5  * 216 = около 6 мм2. Если выбрать кабель меньшего сечения, например, 3 мм2, то на кабеле упадет не 0.5V, а 1V и до устройства дойдет только 11V, кабель будет немного греться, а лента светиться менее ярко.  
**P2**. Пример расчета для электромагнитного замка на 500кг, который находится на расстоянии 15 метров от источника питания. Там ток составляет около 0.5А. Минимальное сечение кабеля будет составлять S = 0.072 * 15  * 0.5 = около 0.5 мм2.  


## Выводы

Система управления QUEEN спроектирована таким образом, что она может быть установлена всегда рядом с квестом, а управление оператором может осуществляться по локальной сети.
Поэтому как правило длины кабельных трасс редко превышают 10-15 метров от системы управления, а значит и источников питания.
На основании этого мы сделали оценочную таблицу, которая без расчетов позволит подобрать нужные сечения кабелей в зависимости от входных параметров:

| Устройство                     | Рекоммендации по кабелю                                                              |
|--------------------------------|--------------------------------------------------------------------------------------|
| audio speaker                  | 2x4.0                                                                                |
| CCTV microphone                | 3x1.5                                                                                |
| CCTV camera                    | специфичный кабель типа IVUE CPV-40AHD, но как правило подставляется в комлекте CCTV |
| elecreomagnetic lock           | 2x1.5                                                                                |
| led strip 5m                   | 2x1.5                                                                                |
| RGB led strip 5m               | 4x1.5                                                                                |
| reeds, buttons, limit switches | 2x0.75                                                                               |
| active sensors, RFID           | 3x1.5                                                                                |
| 12VDC/5VDC power supply        | 2x1.5                                                                                |
| 220/110VAC power supply        | 3x1.5                                                                                |
| Ethernet/RS485                 | FТP/UTP                                                                              |

