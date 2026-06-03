Car Price Prediction — Linear Regression
Практическая работа по анализу данных и построению модели машинного обучения для предсказания цены продажи автомобиля.

Описание проекта
Цель проекта — провести разведочный анализ данных (EDA) о продаже автомобилей и обучить модель линейной регрессии, которая предсказывает цену продажи (`Selling_Price`) на основе характеристик автомобиля.

Датасет
Датасет `car_data.csv` содержит 301 запись и 9 признаков:
Признак	Тип	Описание
`Car_Name`	object	Название автомобиля
`Year`	int64	Год выпуска
`Selling_Price`	float64	Цена продажи (целевая переменная, в лакхах ₹)
`Present_Price`	float64	Текущая рыночная цена (в лакхах ₹)
`Kms_Driven`	int64	Пробег (в км)
`Fuel_Type`	object → int	Тип топлива (Petrol / Diesel / CNG)
`Seller_Type`	object → int	Тип продавца (Dealer / Individual)
`Transmission`	object → int	Тип КПП (Manual / Automatic)
`Owner`	int64	Количество предыдущих владельцев
Пропущенные значения: отсутствуют.

Этапы работы
Импорт библиотек — pandas, matplotlib, seaborn, sklearn
Загрузка и первичный осмотр данных — `.head()`, `.shape`, `.dtypes`
Проверка пропусков — `.isnull().sum()`
Описательная статистика — `.describe()`
Анализ категориальных переменных — распределение по типу топлива, КПП, продавцу
Группировка и агрегация — сравнение Dealer vs Individual
Визуализация — гистограммы, boxplot, scatter plots
Кодирование категориальных переменных — ручное маппирование:
Fuel_Type: `Petrol=0, Diesel=1, CNG=2`
Seller_Type: `Dealer=0, Individual=1`
Transmission: `Manual=0, Automatic=1`
Корреляционная матрица — heatmap через seaborn
Разбивка на train/test — `train_test_split`
Обучение модели — `LinearRegression` из sklearn
Оценка качества — метрики на тестовой выборке

Технологии
Python 3.9
pandas
matplotlib
seaborn
scikit-learn
---
Как запустить
Клонируй репозиторий:
```bash
   git clone https://github.com/<твой-username>/<название-репо>.git
   ```
Установи зависимости:
```bash
   pip install pandas matplotlib seaborn scikit-learn
   ```
Открой ноутбук:
```bash
   jupyter notebook Car_Price_Prediction.ipynb
   ```
Или запусти напрямую в Google Colab.

Автор
Айым Жумабекова
