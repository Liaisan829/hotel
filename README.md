##Hotel Reviews##

###Видео с защитой проекта:


###Папка на Google Drive
https://drive.google.com/drive/folders/1ZooGFY6UlGJWq3L7jNWnp1IQyC_pAsr5

###Датасет
https://www.kaggle.com/datasets/datafiniti/hotel-reviews

Данный датасет - это список из 1000 отелей и их обзоров, предоставленных бизнес-базой данных Datafiniti. Набор данных включает местоположение отеля, название, рейтинг, данные отзывов, название, имя пользователя и многое другое.

###Задача
На основе данных об отелях и отзывах о них найти те параметры, которые влияют на рейтинг больше всего, и вывести способы улучшить его.

###Описания реализованных методов
***Линейная регрессия (Linear regression)*** — модель зависимости переменной x от одной или нескольких других переменных (факторов, регрессоров, независимых переменных) с линейной функцией зависимости.

***Деревья решений (decision trees)***  – это статистический метод, позволяющий предсказывать принадлежность наблюдений или объектов к тому или иному классу категориальной зависимой переменной или среднее значение количественной переменной в зависимости от соответствующих значений одной или нескольких независимых переменных.

***Логистическая регрессия или логит-модель (англ. logit model)*** — статистическая модель, используемая для прогнозирования вероятности возникновения некоторого события путём его сравнения с логистической кривой. Эта регрессия выдаёт ответ в виде вероятности бинарного события (1 или 0).

***Алгоритм случайного леса (Random Forest)*** — универсальный алгоритм машинного обучения, суть которого состоит в использовании ансамбля решающих деревьев. Само по себе решающее дерево предоставляет крайне невысокое качество классификации, но из-за большого их количества результат значительно улучшается. 

***Кластеризация (англ. cluster analysis)*** — это разбиение множества объектов на подмножества (кластеры) по заданному критерию. Каждый кластер включает максимально схожие между собой объекты.

####Кластеризация: алгоритмы k-means и DBSCAN

####Алгоритм k-means (k-средних)

Наиболее простой, но в то же время достаточно неточный метод кластеризации в классической реализации. Он разбивает множество элементов векторного пространства на заранее известное число кластеров k. Действие алгоритма таково, что он стремится минимизировать среднеквадратичное отклонение на точках каждого кластера. Основная идея заключается в том, что на каждой итерации перевычисляется центр масс для каждого кластера, полученного на предыдущем шаге, затем векторы разбиваются на кластеры вновь в соответствии с тем, какой из новых центров оказался ближе по выбранной метрике. Алгоритм завершается, когда на какой-то итерации не происходит изменения кластеров.


####Алгоритм DBSCAN

Это алгоритм кластеризации, основанной на плотности — если дан набор точек в некотором пространстве, алгоритм группирует вместе точки, которые тесно расположены (точки со многими близкими соседями[en]), помечая как выбросы точки, которые находятся одиноко в областях с малой плотностью (ближайшие соседи которых лежат далеко).


###Вывод

Таким образом, наилучшей моделью для предсказания рейтинга отеля на основе данных об отелях стала модель Catboost с результатом на тестовой выборке равным 0.88 коэффициентом детерминации 0.06 (что лучше, чем у линейной регрессии, например)

В качестве решения для улучшения результатов предсказания моделей можно дополнить датасет более точными данными об отелях, такие как количество номеров, звезд и т.д.

###Выполнили

Ахметова Ляйсан 11-004, Терентьева Ольга 11-003
