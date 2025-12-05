### Математика

<details>
<summary>1) Что такое Мультиколлинеарность?</summary>
Это когда несколько признаков линейно зависимы друг от друга. Повышает дисперсию признаков.
</details>

<details>
<summary>2) Чем медиана отличается от среднего?</summary>
</details>

<details>
<summary>3) Что такое квантиль?</summary>
</details>

<details>
<summary>4) Какая вероятность того что при подбрасывании двух шестигранный кубиков выпадет сумма 11?</summary>
</details>

<details>
<summary>5) Теорема Байеса - как выглядет? Как применить?</summary>
</details>

<details>
<summary>6) Что такое p-value и как его обьяснить?</summary>
</details>

<details>
<summary>7) Какие статистические тесты вы знаете и когда их применить?</summary>
</details>

<details>
<summary>8) Отличие дискретной и непрерывной случайной величины?</summary>
</details>

<details>
<summary>9) Что такое закон больших чисел и центральная предельная теорема?</summary>
</details>

<details>
<summary>10) Что такое дисперсия, матожидание, стандартное отклонение и зачем они нужны?</summary>
</details>

<details>
<summary>11) Как понять, что данные распределены нормально?</summary>
</details>

<details>
<summary>12) что такое pdf, cdf?</summary>
</details>


### Разработка

<details>
<summary>1) Что может быть ключом в словаре?</summary>
</details>

<details>
<summary>2) Почему нельзя использовать изменяемый объект как значение по умолчанию?</summary>
</details>

<details>
<summary>3) Как работает сборщик мусора?</summary>
</details>

<details>
<summary>4) Как устроена обработка исключений?</summary>
</details>

<details>
<summary>5) Зачем нужны контекстные менеджеры?</summary>
</details>

<details>
<summary>6) Что такое декоратор?</summary>
</details>

<details>
<summary>7) Как работает наследование?</summary>
</details>

<details>
<summary>8) В чем разница между многопоточностью и параллелизмом?</summary>
</details>

<details>
<summary>9) В чем разница == и is в Python?</summary>
</details>

<details>
<summary>10) Что такое итераторы и зачем они нужны?</summary>
</details>

<details>
<summary>11) Как устроен dict в Python?</summary>
</details>

<details>
<summary>12) Что такое генераторы и как они отличаются от списковых включений?</summary>
</details>

<details>
<summary>13) Чем Docker отличается от Kubernetes?</summary>
</details>

<details>
<summary>14) Чем loc отличается от iloc?</summary>
</details>


### ML

<details>
<summary>1) Как работает логистическая регрессия?</summary>
У нас есть веса признаков, есть обьекты, есть таргеты, мы будет как то обучаться, и чтобы получить ответ модели,транспонированный вектор весов признаков умножается на наш обьект, пропускается через сигмоиду и получаем вероятность принадлежности классу. Оптимизируется лог лосс, почему лог лосс - приходит из теории вероятности из максимизации правдоподибия, он выпуклый, всегда приходим к решению при регуляризации, главная фишка на больших ошибках предсказания - большой штраф.
</details>

<details>
<summary>2) Что такое переобучение и как его заметить?</summary>
Модель слишком сильно подстроилась под данные, на трейне низкая ошибка, на тесте - высокая. (кросс валидация). Есть способы борьбы. Можно добавить шум к данным(дата аугментация).
</details>

<details>
<summary>3) Как найти выбросы?</summary>
</details>

<details>
<summary>4) Как бороться с пропусками?</summary>
</details>

<details>
<summary>5) Какие модели вы знаете?</summary>
</details>

<details>
<summary>6) Какие существуют метрики классификации и регрессии?</summary>
MAE, MSE, MAPE, RMSE.
Recall, precision, accuracy, F1, F-beta, ROC-AUC.
</details>

<details>
<summary>7) Как работает регуляризация с разными моделями?</summary>
</details>

<details>
<summary>8) Что такое гиперпараметры и как подобрать их оптимальные значения?</summary>
</details>

<details>
<summary>9) Что такое дрейф данных, каких видов они бывают и как с ними бороться?</summary>
</details>

<details>
<summary>10) Почему L1 регуляризация зануляет признаки?</summary>
У нас есть гиперплоскость нашего лосса, если мы добавляем L1 регуляризацию, то у нас это получается октаэдр, если L2, то это сфера, а октаэдр сводится к нулям и признаки зануляются. 

Смотрим производную. У L2 идут бОльшие штрафы при бОльших весах, а у L1 модуль более равномерный градиент и поэтому у нас наши веса равномерно отнимаются, а не так чем меньше вес тем меньше ошибка, и получается мы можем сойтись к нулю. 
</details>

<details>
<summary>11) Как устроено дерево решений?</summary>
Бинарное дерево получается, да/нет для категорий, можем разбить числа по бинам
Мы хотим увеличивать прирост информации, а листьях уменьшать дисперсию(критерий gini, MSE)
</details>

<details>
<summary>12) Как бороться с переобучением в деревьях, что такое прунинг?</summary>
можем ограничивать высоту дерева с помощью альфа, прунинг, минимум прирост информации, минимальное количество елементов при обучении, кросс валидация
</details>

<details>
<summary>13) Как работает случайный лес (Random Forest)?</summary>
Бэггинг. Строятся паррально, независимо. Бустрап выборки в данных и в фичах. Варианс уменшается. Выбираем глубокие деревья для низкого байеса.
</details>

<details>
<summary>14) Чем отличается бустинг от Random Forest?</summary>
Бустинг у нас строится последовательно. Каждая модель учится на ошибках предыдущих моделях. Байес уменшает, дисперсию надо уменьшать маленькими моделями.
</details>

<details>
<summary>15) Что такое ROC-AUC и как его интерпретировать?</summary>
ROC показывает если мы берем случайный обьект из класса 1 и из класса 0, то что наша модель их правильно отранжировала.
</details>

<details>
<summary>16) Precision?</summary>
Точность. Сказать формулу, Нас не страшно пропустить хорошие места, но если мы определили хорошее то оно обязано быть хорошим
</details>

<details>
<summary>17) Recall?</summary>
Полнота. Сказать формулу. Важно не пропустить больного, 
</details>

<details>
<summary>18) Связь recall и ROC-AUC?</summary>
Recall используется в рок аук. на осях рок аук на осях для класса 0 и класса 1.
</details>


<details>
<summary>19) Зачем нужна PR-кривая?</summary>
</details>

<details>
<summary>20) Как оценить важность признаков в модели?</summary>
</details>

<details>
<summary>21) Как работать с категориальными фичами?</summary>
</details>

<details>
<summary>22) Как добавить нелинейность в признаки?</summary>
</details>

<details>
<summary>23) Разница между бэггингом и бустингом?</summary>
</details>

<details>
<summary>24) ...</summary>
</details>

<details>
<summary>25) Почему метрика F1 — средняя гармоническая?</summary>
</details>

<details>
<summary>26) Какие бывают усреднения метрик?</summary>
</details>

<details>
<summary>27) Какова взаимосвязь между смещением (bias) и дисперсией (variance)?</summary>
</details>

<details>
<summary>28) Что такое градиентный спуск?</summary>
</details>

<details>
<summary>29) Что такое регуляризация, зачем она нужна и какие есть методы?</summary>
</details>

<details>
<summary>30) Объясните метод главных компонент (PCA)?</summary>
</details>

<details>
<summary>31) Что такое data augmentation? Примеры.</summary>
</details>

<details>
<summary>32) Что такое нормализация данных и зачем она нужна?</summary>
</details>

<details>
<summary>33) Что такое batch normalization и почему оно работает?</summary>
</details>

<details>
<summary>34) Зачем нужны валидационная и тестовая выборка? В чём разница?</summary>
</details>

<details>
<summary>35) Почему ансамбли моделей часто дают лучший результат, чем отдельные модели?</summary>
</details>

<details>
<summary>36) В чём разница между batch gradient descent и stochastic gradient descent?</summary>
</details>

<details>
<summary>37) Что такое линейная зависимость признаков и почему это проблема?</summary>
</details>

<details>
<summary>38) Чем отличаются методы деревьев (Decision Tree, Random Forest, XGBoost, CatBoost)?</summary>
</details>

<details>
<summary>39) Метрики качества для несбалансированных классов?</summary>
</details>


### DL, NLP, LLM

<details>
<summary>1) Функции активации в нейросетях?</summary>
</details>

<details>
<summary>2) Как работает Dropout на inference в нейросетях?</summary>
</details>

<details>
<summary>3) Почему ReLU лучше и чаще используется, чем Sigmoid?</summary>
</details>

<details>
<summary>4) Что такое batch normalization и почему оно работает?</summary>
</details>

<details>
<summary>5) Что такое скорость обучения (learning rate)?</summary>
</details>

<details>
<summary>6) Что такое momentum в оптимизации?</summary>
</details>

<details>
<summary>7) Чем отличаются эпоха, батч и итерация?</summary>
</details>

<details>
<summary>8) Что такое исчезающий и взрывающийся градиент?</summary>
</details>

<details>
<summary>9) Что такое Embeddings и зачем они нужны?</summary>
</details>

<details>
<summary>10) RNN vs LSTM vs GRU — в чём разница?</summary>
</details>

<details>
<summary>11) Attention-механизм — зачем он нужен?</summary>
</details>

<details>
<summary>12) Что такое трансформер?</summary>
</details>

<details>
<summary>13) Что такое токенизация? Какие методы?</summary>
</details>

<details>
<summary>14) Что такое transfer learning и зачем он нужен?</summary>
</details>

<details>
<summary>15) Какие оптимизаторы существуют и как они работают?</summary>
</details>

<details>
<summary>16) Чем эмбединги отличаются от латентного вектора и репрезентаций?</summary>
</details>
