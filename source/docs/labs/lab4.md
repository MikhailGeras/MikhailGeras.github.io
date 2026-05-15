# Лабораторная работа 4. Классификация с применением Scikit-Learn

В работе решалась задача бинарной классификации: прогнозирование дефолта клиента по кредиту.

В основной части были обучены Logistic Regression и Random Forest. Для оценки качества использовались accuracy, confusion matrix, ROC-кривая и ROC-AUC.

В самостоятельной части я дополнительно сравнил kNN, Linear SVM, Extra Trees и HistGradientBoostingClassifier. Лучший результат показала модель HistGradientBoostingClassifier.

Итоговые метрики лучшей модели:

- Accuracy: 0.935973
- ROC-AUC: 0.863742

HistGradientBoostingClassifier немного улучшил результат tuned Random Forest: ROC-AUC вырос с 0.861257 до 0.863742.

Также в работе кратко описано, как обученную модель можно сохранить и подключить к веб-сервису на Flask, Django или FastAPI.

[Открыть ноутбук в Google Colab](https://colab.research.google.com/drive/1ZTr0RoINx9NwUdkJLE4KsPu0uToh7myC?usp=sharing)