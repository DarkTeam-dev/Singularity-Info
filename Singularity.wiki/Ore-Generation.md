# Спавн руд

Руды спавнятся в виде месторождений из 4 руд. Месторождения в среднем занимают площадь 3x3 чанка, высота - всегда 7 блоков. Руды в месторождении всегда подчиняются определённому правилу: каждая руда может спавниться только на своём уровне относительно всего месторождения.

В таблице ниже:
* *Primary Ore* - руда, которая генерируется на высоте с 1 по 3 (начиная сверху относительно месторождения).
* *Secondary Ore* - руда, которая генерируется на высоте с 5 по 7.
* *Inbeween Ore* - руда, которая генерируется на высотах 3 и 4.
* *Sporadic Ore* - руда, которая генерируется на высотах с 1 по 7.
* *Height* - границы высот относительно бедрока, внутри которых генерируется жила.
* *Weight* - вес, вероятность появления жилы.
* *Density* - плотность, числовой параметр, который, чем больше, тем больше блоков руд на единицу объёма.
* *Size* - размер месторождения, чем больше число, тем больую площадь занимает месторождение.

| **Жила**          | **Primary Ore** | **Secondary Ore** | **Inbeween Ore**   | **Sporadic Ore**   | **Height** | **Weight** | **Density** | **Size** |
| ----------------- | --------------- | ----------------- | ------------------ | ------------------ | :--------: | :--------: | :---------: | :------: |
| **Lignite**       | Lignite         | Lignite           | Lignite            | Coal               |   50-130   |    100     |      8      |    32    |
| **Coal**          | Coal            | Coal              | Coal               | Lignite            |   50-80    |     80     |      6      |    32    |
| **Magnetite**     | Magnetite       | Magnetite         | Iron               | Vanadium Magnetite |   50-120   |    160     |      3      |    32    |
| **Gold**          | Magnetite       | Magnetite         | Vanadium Magnetite | Gold               |   60-80    |    160     |      3      |    32    |
| **Iron**          | Brown Limonite  | Yellow Limonite   | Banded Iron        | Malachite          |   10-40    |    120     |      4      |    24    |
| **Cassiterite**   | Tin             | Tin               | Cassiterite        | Tin                |   40-120   |    100     |      5      |    32    |
| **Tetrahedrite**  | Tetrahedrite    | Tetrahedrite      | Copper             | Stibnite           |   80-120   |     70     |      4      |    24    |
| **Nether Quartz** | Nether Quartz   | Nether Quartz     | Nether Quartz      | Nether Quartz      |   40-80    |     80     |      5      |    24    |
| **Sulfur**        | Sulfur          | Sulfur            | Pyrite             | Sphalerite         |   5-20     |    100     |      5      |    24    |
| **Copper**        | Chalcopyrite    | Iron              | Pyrite             | Copper             |   10-30    |     80     |      4      |    24    |
| **Bauxite**       | Bauxite         | Bauxite           | Aluminium          | Ilmenite           |   50-90    |     80     |      4      |    24    |
| **Salts**         | Rock Salt       | Salt              | Lepidolite         | Spodumene          |   50-60    |     50     |      3      |    24    |
| **Redstone**      | Redstone        | Redstone          | Ruby               | Cinnabar           |   10-40    |     60     |      3      |    24    |
| **Soapstone**     | Soapstone       | Talc              | Glauconite         | Pentlandite        |   10-40    |     40     |      3      |    16    |
| **Nickel**        | Garnierite      | Nickel            | Cobaltite          | Pentlandite        |   10-40    |     40     |      3      |    16    |
| **Platinum**      | Sheldonite      | Palladium         | Platinum           | Iridium            |   40-50    |     5      |      3      |    16    |
| **Pitchblende**   | Pitchblende     | Pitchblende       | Uraninite          | Uraninite          |   10-40    |     40     |      3      |    16    |
| **Uranium**       | Uraninite       | Uraninite         | Uranium            | Uranium            |   20-30    |     20     |      3      |    16    |
| **Monazite**      | Bastnasite      | Bastnasite        | Monazite           | Neodymium          |   20-40    |     30     |      3      |    16    |
| **Molybdenum**    | Wulfenite       | Molybdenite       | Molybdenum         | Powellite          |   20-50    |     5      |      3      |    16    |
| **Tungstate**     | Scheelite       | Scheelite         | Tungstate          | Lithium            |   20-50    |     10     |      3      |    16    |
| **Sapphire**      | Almandine       | Pyrope            | Sapphire           | Green Sapphire     |   10-40    |     60     |      3      |    16    |
| **Manganese**     | Grossular       | Spessartine       | Pyrolusite         | Tantalite          |   20-30    |     20     |      3      |    16    |
| **Quartz**        | Quartzite       | Barite            | Certus Quartz      | Certus Quartz      |   40-80    |     60     |      3      |    16    |
| **Diamond**       | Graphite        | Graphite          | Diamond            | Coal               |   5-20     |     40     |      2      |    16    |
| **Olivine**       | Bentonite       | Magnesite         | Olivine            | Glauconite         |   10-40    |     60     |      3      |    16    |
| **Apatite**       | Apatite         | Apatite           | Phosphorus         | Pyrochlore         |   40-60    |     60     |      3      |    16    |
| **Galena**        | Galena          | Galena            | Silver             | Lead               |   30-60    |     40     |      5      |    16    |
| **Lapis**         | Lazurite        | Sodalite          | Lapis              | Calcite            |   20-50    |     40     |      5      |    16    |
| **Beryllium**     | Beryllium       | Beryllium         | Emerald            | Thorium            |   5-30     |     30     |      3      |    16    |
| **Oilsand**       | Oilsand         | Oilsand           | Oilsand            | Oilsand            |   50-80    |     80     |      6      |    32    |
| **Naquadah**      | Naquadah        | Naquadah          | Naquadah           | Naquadah Enriched  |   10-60    |     10     |      5      |    32    |
| **Custom 00**     | Sapphire        | MeteoricIron      | Platinum           | Iridium            |   20-50    |     10     |      2      |    16    |
| **Custom 01**     | Titanium        | Tungsten          | Neodymium          | Vanadium           |   50-120   |     50     |      3      |    16    |
| **Custom 02**     | Graphite        | Ruby              | Desh               | Diamond            |   5-40     |     20     |      2      |    16    |
| **Custom 03**     | Naquadah        | Europium          | Naquadah           | Naquadah           |   10-20    |     10     |      2      |    16    |
| **Custom 04**     | Lutetium        | Naquadah          | Gallium            | Naquadah Enriched  |   20-200   |     30     |      8      |    24    |

Также каждое месторождение спавнится в строго определённых измерениях. Большинство руд доступны для выкапывания в оверворлде.

Доступность месторождений в измерениях:
| **Измерение** | **Всего жил** | **Названия жил** |
| --- | :---: | --- |
| **Overworld** | 29 | Lignite, Coal, Magnetite, Gold, Iron, Cassiterite, Tetrahedrite, Copper, Bauxite, Salts, Redstone, Soapstone, Nickel, Platinum, Pitchblende, Uranium, Monazite, Molybdenum, Tungstate, Sapphire, Manganese, Quartz, Diamond, Olivine, Apatite, Galena, Lapis, Beryllium, Oilsand |
| **Nether** | 8 | Magnetite, Iron, Tetrahedrite, Nether Quartz, Sulfur, Copper, Redstone, Nickel |
| **End** | 8 | Nickel, Platinum, Molybdenum, Tungstate, Manganese, Olivine, Lapis, Beryllium |
| **Moon** | 10 | Gold, Bauxite, Redstone, Uranium, Monazite, Tungstate, Quartz, Olivine, Lapis, Custom 00 |
| **Mars** | 10 | Magnetite, Gold, Iron, Redstone, Platinum, Pitchblende, Monazite, Custom 01, Custom 02, Custom 03 |
| **Asteroids** | 2 | Naquadah, Custom 04 |
