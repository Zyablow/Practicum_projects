# Описание данных

Данные для проекта включают архив объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах за несколько лет. Датасет содержит следующие колонки:
- `airports_nearest` — расстояние до ближайшего аэропорта в метрах (м);
- `balcony` — число балконов;
- `ceiling_height` — высота потолков (м);
- `cityCenters_nearest` — расстояние до центра города (м);
- `days_exposition` — сколько дней было размещено объявление (от публикации до снятия);
- `first_day_exposition` — дата публикации;
- `floor` — этаж;
- `floors_total` — всего этажей в доме;
- `is_apartment` — апартаменты (булев тип);
- `kitchen_area` — площадь кухни в квадратных метрах (м²);
- `last_price` — цена на момент снятия с публикации;
- `living_area` — жилая площадь в квадратных метрах (м²);
- `locality_name` — название населённого пункта;
- `open_plan` — свободная планировка (булев тип);
- `parks_around3000` — число парков в радиусе 3 км;
- `parks_nearest` — расстояние до ближайшего парка (м);
- `ponds_around3000` — число водоёмов в радиусе 3 км;
- `ponds_nearest` — расстояние до ближайшего водоёма (м);
- `rooms` — число комнат;
- `studio` — квартира-студия (булев тип);
- `total_area` — общая площадь квартиры в квадратных метрах (м²);
- `total_images` — число фотографий квартиры в объявлении.

# Задачи проекта

1. **Исследовательский анализ данных:**
   - Изучить общую информацию о датафрейме и построить гистограммы для всех числовых столбцов.
   - Провести предобработку данных, включая заполнение пропущенных значений и изменение типов данных.
   - Устранить неявные дубликаты в столбце с названиями населённых пунктов.

2. **Добавление новых столбцов:**
   - Добавить столбцы с ценой одного квадратного метра, днём недели, месяцем и годом публикации объявления, типом этажа квартиры и расстоянием до центра города в километрах.

3. **Анализ параметров объектов:**
   - Изучить параметры объектов, такие как общая площадь, жилая площадь, площадь кухни, цена объекта, количество комнат, высота потолков, тип этажа квартиры, общее количество этажей в доме, расстояние до центра города и расстояние до ближайшего парка.
   - Построить гистограммы для каждого параметра, удалив редкие и выбивающиеся значения.

4. **Анализ времени продажи:**
   - Изучить, как быстро продавались квартиры, построить гистограмму, посчитать среднее и медиану времени продажи.
   - Определить, какие продажи можно считать быстрыми, а какие — необычно долгими.

5. **Факторы, влияющие на стоимость:**
   - Определить факторы, которые больше всего влияют на общую стоимость объекта.
   - Изучить зависимость цены от общей площади, жилой площади, площади кухни, количества комнат, этажа, на котором расположена квартира, и даты размещения объявления.
   - Построить графики, показывающие зависимость цены от этих параметров.

6. **Средняя цена квадратного метра:**
   - Посчитать среднюю цену одного квадратного метра в 10 населённых пунктах с наибольшим числом объявлений.
   - Выделить населённые пункты с самой высокой и низкой стоимостью квадратного метра.

7. **Зависимость стоимости от расстояния до центра:**
   - Выделить квартиры в Санкт-Петербурге и вычислить их среднюю стоимость на разном удалении от центра.
   - Построить график изменения средней цены для каждого километра от центра Петербурга.

8. **Общий вывод:**
   - Описать полученные результаты и зафиксировать итоговый вывод проведённого исследования.

---

# Data Description

The data for the project includes an archive of apartment sale listings in St. Petersburg and neighboring localities over several years. The dataset contains the following columns:
- `airports_nearest` — distance to the nearest airport in meters (m);
- `balcony` — number of balconies;
- `ceiling_height` — ceiling height (m);
- `cityCenters_nearest` — distance to the city center (m);
- `days_exposition` — number of days the listing was posted (from publication to removal);
- `first_day_exposition` — publication date;
- `floor` — floor number;
- `floors_total` — total number of floors in the building;
- `is_apartment` — apartment (boolean type);
- `kitchen_area` — kitchen area in square meters (m²);
- `last_price` — price at the time of removal from publication;
- `living_area` — living area in square meters (m²);
- `locality_name` — name of the locality;
- `open_plan` — open floor plan (boolean type);
- `parks_around3000` — number of parks within a 3 km radius;
- `parks_nearest` — distance to the nearest park (m);
- `ponds_around3000` — number of bodies of water within a 3 km radius;
- `ponds_nearest` — distance to the nearest body of water (m);
- `rooms` — number of rooms;
- `studio` — studio apartment (boolean type);
- `total_area` — total area of the apartment in square meters (m²);
- `total_images` — number of photos of the apartment in the listing.

# Project Tasks

1. **Exploratory Data Analysis:**
   - Study the general information about the dataframe and build histograms for all numerical columns.
   - Perform data preprocessing, including filling in missing values and changing data types.
   - Eliminate implicit duplicates in the column with locality names.

2. **Adding New Columns:**
   - Add columns with the price per square meter, day of the week, month, and year of the listing publication, type of apartment floor, and distance to the city center in kilometers.

3. **Parameter Analysis:**
   - Study the parameters of the objects, such as total area, living area, kitchen area, object price, number of rooms, ceiling height, type of apartment floor, total number of floors in the building, distance to the city center, and distance to the nearest park.
   - Build histograms for each parameter, removing rare and outlier values.

4. **Sales Time Analysis:**
   - Study how quickly apartments were sold, build a histogram, calculate the mean and median sales time.
   - Determine which sales can be considered fast and which are unusually slow.

5. **Factors Affecting Price:**
   - Identify the factors that most influence the total price of the object.
   - Study the dependence of price on total area, living area, kitchen area, number of rooms, floor on which the apartment is located, and the date of the listing publication.
   - Build graphs showing the dependence of price on these parameters.

6. **Average Price per Square Meter:**
   - Calculate the average price per square meter in the 10 localities with the highest number of listings.
   - Identify localities with the highest and lowest cost per square meter.

7. **Price Dependence on Distance to the Center:**
   - Identify apartments in St. Petersburg and calculate their average price at different distances from the center.
   - Build a graph of the change in average price for each kilometer from the center of St. Petersburg.

8. **General Conclusion:**
   - Describe the obtained results and document the final conclusion of the conducted research.