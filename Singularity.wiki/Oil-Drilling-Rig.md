**По-русски**: Буровая установка, установка для бурения нефтяных скважин.

# Oil Drilling Rig
Многоблочная машина для выкачивания подземной воды, нефти или природного газа.<br>
Состав:
* Oil Drilling Rig (контроллер, нижний слой)
* Output Hatch (нижний слой)
* Energy Hatch (нижний слой)
* Maintenance Hatch (1 шт, нижний слой)
* Machine Casing (от 3 до 8)
* Frame Box (15 шт.)
* Input Bus (не обязательно, нижний слой)
* Output Bus (не обязательно, нижний слой)

Oil Drilling Rig требует буровые трубы для бурения скважины до бедрока или нулевой высоты. После чего начинает подавать найденную жидкость в Output Hatch. Конфигурационные платы (Programmed Circuit) позволяют завершить работу установки при достижении объёма жижи, равному сумме значений всех плат. Соответственно, по-умолчанию без плат качалка будет работать до полного опустошения месторождения.

Существует 3 вида буровых установок: Oil Drilling Rig I, Oil Drilling Rig II, Oil Drilling Rig III, которые различаются активной площадью выкачивания.

| * | Oil Drilling Rig I | Oil Drilling Rig II | Oil Drilling Rig III |
| --- | :---: | :---: | :---: |
| Площадь выкачивания | 1 чанк | 3x3 чанка | 6x6 чанков |
| Минимальный энерготир | MV | HV | EV |
| Потребление на начальном энерготире, еу/т | 48 | 192 | 768 |
| Длительность 1 операции выкачивания, т | 80 | 40 | 20 |
| Frame Box | Steel Frame Box | Titanium Frame Box | Tungstensteel Frame Box |
| Machine Casing | Solid Steel Machine Casing | Stable Titanium Machine Casing | Robust Tungstensteel Machine Casing |
| Фото | ![ODR1](https://raw.githubusercontent.com/IdealIndustrial/IdealIndustrial.github.io/main/wiki/odr1.jpg) | ![ODR2](https://raw.githubusercontent.com/IdealIndustrial/IdealIndustrial.github.io/main/wiki/odr2.jpg) | ![ODR3](https://raw.githubusercontent.com/IdealIndustrial/IdealIndustrial.github.io/main/wiki/odr3.jpg) |

Повышение тира Energy Hatch'а позволяет увеличить суммарный объём выкаченной жидкости за счёт того, что в Output Hatch будет поставляться больше жидкости, а объём потребления месторождения останется прежним.

Oil Drilling Rig качает весь квадрат своей сетки всегда
* ODR1 всегда качает чанк, в котором стоит;
* ODR2 всегда качает ту четверть спота, в которой стоит (все 9 чанков и вне зависимости в каком из 9 она стоит);
* ODR3 всегда качает тот спот, в котором стоит (все 36 чанков вне зависимости от конкретного чанка).

В мире располагаются невидимые месторождения подземных жидкостей. Каждое месторождение имеет одинаковую площадь размером в 6 на 6 чанков. Жидкости есть в Оверворлде, Незере и на Луне.

## Таблицы генерации подземных жидкостей по каждому измерению
Min Amoun - минимальный объём  
Max Amount - максимальный объём  
Decrease Per Operation Amount - actual fluid gained works like (Litre)VeinData/5000.  
Chance - вероятность нахождения.

### Overworld
| Название | Min Amoun | Max Amount | Decrease Per Operation Amount | Chance |
| --- | :---: | :---: | :---: | :---: |
| Пусто | - | - | - | 50 |
| Вода | 200 | 2000 | 1 | 30 |
| Natural Gas | 90 | 625 | 7 | 4 |
| Light Oil | 90 | 625 | 6 | 4 |
| Raw Oil | 90 | 625 | 5 | 4 |
| Oil | 90 | 625 | 5 | 4 |
| Heavy Oil | 90 | 625 | 4 | 4 |

Примечание: конфигурация ИИС предусматривает количество пустых областей без жидкостей в районе 50%. Также за счёт высокой частоты генерации воды, чаще попадается вода, чем нефть. Найти нефть может быть сложно. Потому используйте [Seismic Prospector](https://github.com/IdealIndustrial/GT5Unofficial/wiki/Seismic-Prospector).<br>

### Nether
| Название | Min Amoun | Max Amount | Decrease Per Operation Amount | Chance |
| --- | :---: | :---: | :---: | :---: |
| Пусто | - | - | - | 50 |
| Лава | 500 | 1000 | 1 | 20 |
| H2S | 400 | 800 | 1 | 10 |
| Ртуть | 300 | 600 | 1 | 10 |
| Molten Redstone | 10 | 40 | 1 | 5 |
| Molten Gold | 2 | 6 | 1 | 5 |

### Луна
| Название | Min Amoun | Max Amount | Decrease Per Operation Amount | Chance |
| --- | :---: | :---: | :---: | :---: |
| Пусто | - | - | - | 75 |
| Гелий 3 | 50 | 150 | 1 | 25 |
