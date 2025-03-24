# Sale-of-apartments
Исследование объявлений о продаже квартир

## Описание проекта 
В распоряжении есть данные сервиса Яндекс Недвижимость — архив объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах за несколько лет. Нужно определить рыночную стоимость объектов недвижимости. Для этого провести исследовательский анализ данных и установите параметры, влияющие на цену объектов. Это позволит построить автоматизированную систему: она отследит аномалии и мошенническую деятельность.
По каждой квартире на продажу доступны два вида данных. Первые вписаны пользователем, вторые — получены автоматически на основе картографических данных. Например, расстояние до центра, аэропорта и других объектов — эти данные автоматически получены из геосервисов. Количество парков и водоёмов также заполняется без участия пользователя.

## Описание данных
- airports_nearest — расстояние до ближайшего аэропорта в метрах (м);
- balcony — число балконов;
- ceiling_height — высота потолков (м);
- cityCenters_nearest — расстояние до центра города (м);
- days_exposition — сколько дней было размещено объявление (от публикации до снятия);
- first_day_exposition — дата публикации;
- floor — этаж;
- floors_total — всего этажей в доме;
- is_apartment — апартаменты (булев тип);
- kitchen_area — площадь кухни в квадратных метрах (м²);
- last_price — цена на момент снятия с публикации;
- living_area — жилая площадь в квадратных метрах (м²);
- locality_name — название населённого пункта;
- open_plan — свободная планировка (булев тип);
- parks_around3000 — число парков в радиусе 3 км;
- parks_nearest — расстояние до ближайшего парка (м);
- ponds_around3000 — число водоёмов в радиусе 3 км;
- ponds_nearest — расстояние до ближайшего водоёма (м);
- rooms — число комнат;
- studio — квартира-студия (булев тип);
- total_area — общая площадь квартиры в квадратных метрах (м²);
- total_images — число фотографий квартиры в объявлении
  
## Инструменты:
`Python`
`Matplotlib`
`Seaborn`

## Общий вывод
Чаще всего на продажу выставляются квартиры с общей площадью 35-45 м2, с жилой площадью 18 м2 и 32 м2, площадью кухни около 10 м2. Высота потолков - 2,65 м. Цены на квартиры варьируются в районе 3,4-4,5 миллионов. Много квартир с 1-2 комнатами, на которые традиционно всегда большой спрос. Квартир не на первом и не на последнем этаже больше остальных. Чем дальше от центра, тем больше квартир на продажу, много предложение в спальных районах, удаленных от центра. Продажа квартиры в среднем занимает около месяца. Слишком быстрыми продажами можно считать продажи, не превышающие одного месяца (несколько недель или даже дней), необычно долгими - от года и больше.

Цена на квартиру сильно зависит от общей площади квартиры, жилой площади, площади кухни, количества комнат в квартире: чем эти показатели выше, тем и цена будет больше. Зависимость существуется также между ценой квартиры и этажом: меньше стоимость квартир на первом и последнем этажах. Небольшая отрицательная корреляция есть между годом и ценой: с 2015 по 2018 годы наблюдалось падение цены. Недвижимость дороже в Санкт-Петербурге, чем за его пределами: с удалением от города уменьшается и цена.
