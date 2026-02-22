# Огород на жёрдочках

## Бонусы от биомов

В игре все биомы имеют ряд признаков, описывающих температуру, природу, тип биома. Так, к примеру, биому Cold Taiga соответствуют признаки COLD, CONIFEROUS, FOREST, SNOWY. Всего используется 26 признаков: BEACH, COLD, CONIFEROUS, DEAD, DENSE, DRY, END, FOREST, HILLS, HOT, JUNGLE, MESA, MOUNTAIN, MUSHROOM, NETHER, OCEAN, PLAINS, RIVER, SANDY, SAVANNA, SNOWY, SPARSE, SPOOKY, SWAMP, WASTELAND, WET. Так как биомы могут называться по-разному, называться разными языками или иметь множество вариаций, удобно контролировать некоторые параметры через эти указанные признаки.

Влажность и питательность почвы привязаны к признакам биомов и имеют числовые значения. Эти числа называются бонусами влажности и питательности, соответственно. Они прописаны вручную:

|   | Бонус влажности | Бонус питательности |
| --- | --- | --- |
| JUNGLE | 7 | 10 |
| SWAMP | 10 | 10 |
| MUSHROOM | 5 | 5 |
| FOREST | 5 | 5 |
| RIVER | 10 | 2 |
| PLAINS | 2 | 0 |
| SAVANNA |  | -2 |
| HILLS |  | -5 |
| MOUNTAIN |  | -5 |
| WASTELAND |  | -8 |
| END |  | -10 |
| NETHER |  | -10 |
| DEAD |  | -10 |

Когда биом имеет несколько признаков из таблицы бонусов, бонусы не складываются, а берётся максимальное значение.

Например, биом JungleHills помечен тегами HOT, DENSE, WET, JUNGLE, HILLS. По таблице бонусов видим, что JUNGLE имеет бонус питательности +10 и HILLS имеет бонус питательности -5. Из этих двух чисел +10 и -5 конечным бонусом питательности почвы станет +10, как наибольшее.

Из-за бага в IC2 отрицательные бонусы не учитываются, и считается, что их нету. Потому огород будет расти одинаково, что на Луне, что в Пустыне, что в холодной тайге, что в океане.

| **Название биома**   | Бонус влажности | Бонус питательности | **Признаки**                           |
| -------------------- | :-------------: | :-----------------: | -------------------------------------- |
| asteroids            | 0               | 0                   | COLD, DRY, SPOOKY, DEAD                |
| Beach                | 0               | 0                   | BEACH                                  |
| Birch Forest         | 5               | 5                   | FOREST                                 |
| Birch Forest Hills   | 5               | 5                   | FOREST, HILLS                          |
| Birch Forest Hills M | 0               | 0                   | HILLS                                  |
| Birch Forest M       | 0               | 0                   | HILLS                                  |
| Cold Beach           | 0               | 0                   | COLD, SNOWY, BEACH                     |
| Cold Taiga           | 5               | 5                   | COLD, CONIFEROUS, FOREST, SNOWY        |
| Cold Taiga Hills     | 5               | 5                   | COLD, CONIFEROUS, FOREST, HILLS, SNOWY |
| Cold Taiga M         | 0               | 0                   | COLD, HILLS, SNOWY                     |
| Deep Ocean           | 0               | 0                   | OCEAN                                  |
| Desert               | 0               | 0                   | HOT, DRY, SANDY                        |
| Desert M             | 2               | 0                   | HOT, DRY, PLAINS, SANDY                |
| DesertHills          | 0               | 0                   | HOT, DRY, HILLS, SANDY                 |
| Extreme Hills        | 0               | 0                   | MOUNTAIN, HILLS                        |
| Extreme Hills Edge   | 0               | 0                   | MOUNTAIN                               |
| Extreme Hills M      | 0               | 0                   | HILLS                                  |
| Extreme Hills+       | 5               | 5                   | SPARSE, FOREST, MOUNTAIN               |
| Extreme Hills+ M     | 0               | 0                   | HILLS                                  |
| Flower Forest        | 5               | 5                   | FOREST, HILLS                          |
| Forest               | 5               | 5                   | FOREST                                 |
| ForestHills          | 5               | 5                   | FOREST, HILLS                          |
| FrozenOcean          | 0               | 0                   | COLD, OCEAN, SNOWY                     |
| FrozenRiver          | 10              | 2                   | COLD, RIVER, SNOWY                     |
| Hell                 | 0               | 0                   | HOT, DRY, NETHER                       |
| Ice Mountains        | 0               | 0                   | COLD, MOUNTAIN, SNOWY                  |
| Ice Plains           | 0               | 0                   | COLD, SNOWY, WASTELAND                 |
| Ice Plains Spikes    | 0               | 0                   | COLD, HILLS, SNOWY                     |
| Jungle               | 7               | 10                  | HOT, DENSE, WET, JUNGLE                |
| Jungle M             | 0               | 0                   | HOT, WET, HILLS                        |
| JungleEdge           | 7               | 10                  | HOT, WET, JUNGLE, FOREST               |
| JungleEdge M         | 0               | 0                   | HOT, HILLS                             |
| JungleHills          | 7               | 10                  | HOT, DENSE, WET, JUNGLE, HILLS         |
| marsFlat             | 0               | 0                   | COLD, DRY, DEAD, SANDY                 |
| Mega Spruce Taiga    | 5               | 5                   | DENSE, FOREST                          |
| Mega Spruce Taiga    | 5               | 5                   | DENSE, FOREST                          |
| Mega Taiga           | 5               | 5                   | COLD, CONIFEROUS, FOREST               |
| Mega Taiga Hills     | 5               | 5                   | COLD, CONIFEROUS, FOREST, HILLS        |
| Mesa                 | 0               | 0                   | MESA, SANDY                            |
| Mesa (Bryce)         | 2               | 0                   | HOT, DRY, PLAINS, SANDY                |
| Mesa Plateau         | 0               | 0                   | MESA, SANDY                            |
| Mesa Plateau F       | 0               | 0                   | SPARSE, MESA, SANDY                    |
| Mesa Plateau F M     | 5               | 5                   | HOT, DRY, FOREST, SANDY                |
| Mesa Plateau M       | 2               | 0                   | HOT, DRY, PLAINS, SANDY                |
| moon                 | 0               | 0                   | COLD, DRY, DEAD                        |
| MushroomIsland       | 5               | 5                   | MUSHROOM                               |
| MushroomIslandShore  | 5               | 5                   | MUSHROOM, BEACH                        |
| Ocean                | 0               | 0                   | OCEAN                                  |
| Plains               | 2               | 0                   | PLAINS                                 |
| River                | 10              | 2                   | RIVER                                  |
| Roofed Forest        | 5               | 5                   | DENSE, SPOOKY, FOREST                  |
| Roofed Forest M      | 0               | 0                   | HILLS                                  |
| Savanna              | 2               | 0                   | HOT, SPARSE, SAVANNA, PLAINS           |
| Savanna M            | 0               | 0                   | HOT, SPARSE, DRY, SAVANNA, HILLS       |
| Savanna Plateau      | 2               | 0                   | HOT, SPARSE, SAVANNA, PLAINS           |
| Savanna Plateau M    | 0               | 0                   | HOT, SPARSE, DRY, SAVANNA, HILLS       |
| Sky                  | 0               | 0                   | COLD, DRY, END                         |
| space                | 2               | 0                   | DRY, PLAINS                            |
| Stone Beach          | 0               | 0                   | BEACH                                  |
| Storage Cell         | 2               | 0                   | COLD, PLAINS                           |
| Sunflower Plains     | 2               | 0                   | PLAINS                                 |
| Swampland            | 10              | 10                  | WET, SWAMP                             |
| Swampland M          | 10              | 10                  | WET, SWAMP                             |
| Taiga                | 5               | 5                   | COLD, CONIFEROUS, FOREST               |
| Taiga M              | 0               | 0                   | HILLS                                  |
| TaigaHills           | 5               | 5                   | COLD, CONIFEROUS, FOREST, HILLS        |