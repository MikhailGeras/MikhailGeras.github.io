# Лабораторная работа 5. Регрессия с применением Scikit-Learn

В работе решалась задача регрессии: нужно было предсказать цену недвижимости по характеристикам объекта.

В основной части были обучены Linear Regression и Random Forest Regressor. Для оценки качества использовались MAE, MSE и RMSE.

В самостоятельной части я проверил удаление слабых признаков, подобрал параметры Random Forest и сравнил дополнительные модели регрессии: RidgeCV, LassoCV, Extra Trees, Gradient Boosting и HistGradientBoostingRegressor.

Лучший результат показала модель HistGradientBoostingRegressor.

Итоговые метрики лучшей модели:

- MAE: 67889.44
- RMSE: 122351.79

По сравнению с базовым Random Forest RMSE уменьшился с 135516.61 до 122351.79.

Также в работе описано, как обученную модель можно сохранить и подключить к веб-сервису на Flask, Django или FastAPI.

[Открыть ноутбук в Google Colab](https://colab.research.google.com/drive/1ZhXoRjRq8PibVp4bU50d5omYSPIIazvB?usp=sharing)