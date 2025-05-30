# Прогнозирование покупательской активности для интернет-магазина

## Описание проекта
Проект разработан для интернет-магазина с целью предотвращения снижения покупательской активности постоянных клиентов. Решение включает:

1. **Прогнозную модель** для определения вероятности снижения активности
2. **Сегментацию клиентов** для персонализированных предложений
3. **Рекомендации** по удержанию ценных покупателей

## Задача
Разработать систему персонализации предложений на основе:
- Анализа поведения клиентов
- Прогноза изменения активности
- Оценки прибыльности каждого покупателя

## Данные
Проект использует 4 источника данных:
1. `market_file.csv` - основная информация о клиентах и их поведении
2. `market_money.csv` - данные о выручке по периодам
3. `market_time.csv` - время на сайте по периодам  
4. `money.csv` - прибыль от клиентов

## Методология
### 1. Предобработка данных
- Объединение таблиц
- Очистка и преобразование данных
- Фильтрация активных клиентов (≥3 месяцев)

### 2. Анализ и моделирование
- Корреляционный анализ признаков
- Построение 4 моделей классификации:
  - KNN
  - Decision Tree
  - Logistic Regression
  - SVM
- Оценка важности признаков (SHAP)

### 3. Сегментация и рекомендации
- Кластеризация клиентов
- Анализ ключевых сегментов
- Разработка персонализированных стратегий
