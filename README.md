# Yandex-Practicum-projects

Репозиторий в основном содержит учебно-практические проекты, выполненные в рамках курса яндекс.практикума.

Проекты выполнены на питоне, в них продемонстрированы мои навыки в очистке, предобработке, исследовательском анализе, проверке статистических гипотез, расчёте и анализе бизнес-метрик, когортном анализе, интерпретации результатов A/A/B тестирования.

При анализе данных используются библиотеки pandas, numpy, matplotlib, sns, statistics и другие.

Список и описание выполненных проектов:

**1. Приоритизация гипотез и анализ A/B-теста интернет-магазина**

Ссылка: https://github.com/Anargasanov/Yandex-Practicum-projects/blob/79e362b09c1dc5330fd50cc7cbcb6916d1a5605a/AB-testing/AB_testing_hypothesis.ipynb

Определены приоритетные гипотезы из 9 предложенных с помощью фреймворков приоритизации (RICE и ICE). Проанализирован A/B тест интернет магазина с целью проверки гипотез, включающий в себя:

- предобработку данных (логов с заказами пользователей и информацией о количестве посетителей интернет-магазина по датам за месяц);
- аналитическую оценку данных (сбор кумулятивных метрик: выручка по группам A/B теста, средний чек и его относительное изменение, конверсия и ее относительное изменение, количество заказов по пользователям, стоимость заказов);
- визуализацию полученных метрик и написание выводов;
- расчет статистической значимости различий в метриках по группам A/B-теста (с очищенными от выбросов данными и неочищенными);
- проверку гипотез об отсутствии статистически значимых различий в конверсии и об отсутствии различий в стоимости среднего чека между группами критерием Манна-Уитни;
- описание выводов по проведенному анализу A/B-теста, было определно, что дальнейшее проведение теста нецелесообразно, так как подтвердилось наличие статистически значимых различий по конверсии и отсутствие по среднему чеку.

Стек инструментов: python, pandas, matplotlib, seaborn, scipy, фреймворки приоритизации гипотез (RICE, ICE), A/B-тестирование, статистический тест

**2. Исследование надёжности заёмщиков кредитного отдела банка**

<code>[Ссылка](https://github.com/Anargasanov/Yandex-Practicum-projects/blob/79e362b09c1dc5330fd50cc7cbcb6916d1a5605a/Banking-data/bank_clients.ipynb)
</code>
Ссылка: https://github.com/Anargasanov/Yandex-Practicum-projects/blob/79e362b09c1dc5330fd50cc7cbcb6916d1a5605a/Banking-data/bank_clients.ipynb

Изучена исходная информация (данные со статистикой о платежеспособности клиентов банка, где имеются характеристики клиентов и булевый столбец имеет просрочки по погашению или нет), в данном проекте продемонстрированы глубокие навыки предобработки данных. Выполнена преобработка данных (обработаны пропуски, заменены типы данных, обработаны дубликатов, удалены неявные дубликаты характеристик при помощи лемматизатора, категоризированы данные при помощи метода расчета квартилей). Интерпретированы результаты и получены ответы на поставленные вопросы исследования.

Стек инструментов: python, pandas, mystem (лемматизатор), matplotlib, описательная статистика

**3. Анализ данных интернет-магазина игр (изучение закономерностей определяющих успешность видеоигр)**

Сссылка: https://github.com/Anargasanov/Yandex-Practicum-projects/blob/79e362b09c1dc5330fd50cc7cbcb6916d1a5605a/Game-shop/gameshop.ipynb

Дана первичная оценка историческим данным, выполнена предобработка (приведение столбцов к нужным типам, обработаны дубликаты, обработаны пропуски, расчитаны столбцы с общими продажами). Проведен исследовательский анализ данных (EDA), выбран актуальный период анализа, проанализировано изменение продаж по платформам, изучено распределение игр по жанрам, изучена корреляция между отзывами и продажами, построен график жизненного цикла платформ, построены портреты пользователей по рассматриваемым регионам, определены популярные платформы и жанры для каждого региона, рассмотрено влияние возрастного рейтинга на популярность игр. Проверены гипотезы с помощью t-теста для несвязных выборок: средние пользовательские рейтинги платформ Xbox One и PC одинаковые; средние пользовательские оценки жанров Action и Sports имеют статистически значимое различие. Собран общий вывод по анализу и даны прогнозные рекомендации по наиболее потенциально прибыльным платформам и жанрам.

Стек инструментов: python, pandas, numpy, scipy, статистический тест, matplotlib, seaborn, описательная статистика

**4. Анализ пользовательского поведения приложения по продаже продуктов питания**

Ссылка: https://github.com/Anargasanov/Yandex-Practicum-projects/blob/79e362b09c1dc5330fd50cc7cbcb6916d1a5605a/Grocery-shop/project_shop_app.ipynb

Проведена событийная аналитика. На основе логов пользователей построена воронка продаж, исследован путь пользователей от авторизации в приложении до покупки. Проанализированы результаты A/A/B-теста по введению новых шрифтов. Проведено сравнение контрольных групп при помощи Z-теста для расчета разницы между пропорциями в наблюдаемых выборках из генеральной совокупности. Проведены множественные сравнения между контрольными и экспериментальной группами с поправкой Бонферрони для выявления статистически значимых различий между выборками. По результатам эксперимента выявлено, что статистически значимые различия между группами отсутствуют, новый шрифт не повлияет на увеличение конверсии.

Стек инструментов: python, pandas, numpy, scipy, статистический тест, A/B-тестирование, A/A-тестирование, matplotlib, plotly, seaborn, продуктовые метрики

**5. Анализ убыточности маркетинговой кампании приложения**

Ссылка: https://github.com/Anargasanov/Yandex-Practicum-projects/blob/79e362b09c1dc5330fd50cc7cbcb6916d1a5605a/Marketing-analysis/unit_economics_cohorts.ipynb

На основе логов сервера с данными о посещениях и покупках в приложении новыми пользователями за пол года проведен анализ маркетинговой кампании. Написаны функции для расчета и визуализации бизнес-метрик (LTV, ROI, удержание, конверсия), проведен исследовательский анализ данных (определена географическая принадлежность новых пользователей, типы устройств, рекламные каналы в разрезе платящих и неплатящих пользователей), проанализированы затраты на маркетинг в исследуемый период (acquisition costs), проведен когортный анализ по написанным функциям создания профилей пользователей и расчета бизнес-метрик, проанализирована окупаемость рекламы с разбивкой по различным характеристикам пользователей, описаны выводы и даны рекомендации.

Стек инструментов: python, pandas, matplotlib, seaborn, когортный анализ, юнит-экономика, продуктовые метрики

**6. Анализ рынка недвижимость Санкт-Петербурга (объявления о продаже квартир сервиса Яндекс.Недвижимость)**

Ссылка: https://github.com/Anargasanov/Yandex-Practicum-projects/blob/79e362b09c1dc5330fd50cc7cbcb6916d1a5605a/Real-estate/real_estate.ipynb

Проведена предобработка данных, заполнены пропуски, определена рыночная стоимость объектов недвижимости разного типа в зависимости от характеристик квартир (высота потолков, количество комнат, жилая площадь, удаленность от центра). Дана оценка влияния факторов на стоимость квартир в Санкт-Петербурге, все выводы визуализированы, использованы различные виды графиков (боксплоты, диаграммы размаха, диаграммы частот, линейные графики и проч.). Сделаны выводы о факторах, влияющих на стоимость недвижимости.

Стек инструментов: python, pandas, matplotlib, описательная статистика, категоризация переменных

**7. Исследования рынка общепита в Москве для принятия решения об открытии нового заведения**

Ссылка: https://github.com/Anargasanov/Yandex-Practicum-projects/blob/79e362b09c1dc5330fd50cc7cbcb6916d1a5605a/Restaurants-Moscow/restaurants_moscow.ipynb

На основе данных заведениях общественного питания города Москвы проведен анализ типов объектов, их расположения, количества посадочных мест, принадлежность ресторана к сетевому типу распространения). Проведен исследовательский анализ и даны рекомендации о характеристиках заведения и дана оценка возможности развития сети.

Стек инструментов: python, pandas, matplotlib, plotly, google презентации
