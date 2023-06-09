<h2 style = "text-align:center;
             font-size:30px;"> Введение </h2>
             
Работа Слепцова Гаврила по прогнозированию цены б/у машин с использованием catboost.

<h2 style = "text-align:center;
             font-size:30px;"> Описание задачи </h2>
    
Перед нами стоит задача предсказать стоимость б/у автомобиля и проверить нашу модель на тестовой выборке. Мы будем использовать метрику MAPE (Mean Absolute Percentage Error) и стремиться достичь минимального значения.

![MAPE](https://www.googleapis.com/download/storage/v1/b/kaggle-user-content/o/inbox%2F452676%2F99bf86af22241438a654f7e8eecf294e%2F2023-03-20%20%2017.16.01.png?generation=1679314590278751&alt=media)

Работа выполнена в рамках конкурса Kaggle: https://www.kaggle.com/competitions/used-cars-price-prediction/leaderboard

<h2 style = "text-align:center;
             font-size:30px;"> Описание данных </h2>

Датасет содержит следующие признаки:

- 'year' - год производства автомобиля;
- 'make' - производитель автомобиля;
- 'model' - модель автомобиля;
- 'trim' - модификация автомобиля;
- 'body' - тип кузова автомобиля;
- 'transmission' - тип КПП;
- 'vin' - идентификатор (вин) автомобиля;
- 'state' - штат регистрации автомобиля;
- 'condition' - состояние автомобиля по шкале от 1 до 5;
- 'odometer' - пробег автомобиля в милях;
- 'color' - цвет кузова автомобиля;
- 'interior' - цвет интерьера автомобиля;
- 'seller' - продавец автомобиля;
- 'saledate' - дата продажи автомобиля.

Целевым признаком является 'sellingprice' - стоимость продажи автомобиля.

<h2 style = "text-align:center;
             font-size:30px;"> План работы </h2>
    
1. Загрузка и предобработка данных.
2. Обучение различных моделей:
- CatBoost;
- LightGBM;
- Random Forest;
- Линейные модели;
- KNeighbors;
- Голосование (Voting).
3. Выбор наилучшей модели.
4. Анализ влияния различных параметров на результат.
5. Выполнение прогноза для тестовой выборки.
