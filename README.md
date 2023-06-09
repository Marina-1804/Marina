# Марина
# Обо мне
Привет! Меня зовут Марина, я начинающий аналитик данных. В этом репозитории вы можете найти некоторые из моих проектов, выполненных во время обучения и практики.

# Навыки и технологии
Инструменты анализа данных: SQL, Excel

Системы управления базами данных: PostgreSQL

# Проекты
Проект 1: **Калькулятор юнит-экономики онлайн-школы**

Что нужно было сделать:

В ходе работы необходимо было рассмотреть несколько способов, которыми можно было увеличить маржу или лояльность сотрудников:

- на сколько компания может увеличить траты на ЗП сотрудников, при этом сохранив маржинальность в допустимых пределах;
- как сильно мы сможем увеличить маржинальность, перераспределив доли платных и бесплатных уроков;
- на сколько увеличатся в среднем наши доходы, если мы сможем лучше "удерживать" студентов.

Как решала: 
- исходя из предпологаемой маржинальности рассчитала ФОТ;
- посчитала доли уроков разной цены, долю бесплатных уроков, рассчитала выручку при новых условиях,учитывая изменения, рассчитала маржинальность;
- пересчитала Lifetime, LTRю , долю расходов на привлечение %CAC, получила новую маржинальность.

Ссылка на проект (прикладываю скриншоты результатов работы,т. к. данные конфеденциальны):

https://drive.google.com/file/d/1R2_nui_DEwgdiEiKBg6X0ejz-NHtA65N/view?usp=sharing

https://drive.google.com/file/d/1s9bbG_oUS7u18E5-M6xym3vMIfPZvB_1/view?usp=sharing

https://drive.google.com/file/d/1s-0bliuXMVmPb4H1-m94E_9In0Ud98-X/view?usp=sharing

Выводы:

На основании данных, полученных от работодателя были выполнены перерасчеты, в результате которых получили маржинальность проекта при различных условиях.

Проект 2: **Калькулятор юнит-экономики онлайн-кинотеатра**

Целью работы было узнать, насколько эффективно работает онлайн-кинотеатр и предложить варианты для улучшения ситуации, для этого было необходимо:
- посчитать юнит-экономику продукта;
- предложить сценарий по настройке параметров для выхода на 25-процентную маржинальность;
- собрать наглядную визуализацию

Как решала: 
- рассчитала необходимые для дальнейшей работы метрики; 
- подогнала параметры таким образом, чтобы маржинальность была +25%; 
- построила необходимые графики.

Ссылка на проект:

https://docs.google.com/presentation/d/1U80E1uWVe68SOl8wRHZ9ToOcHP95RFd5/edit?usp=sharing&ouid=118221966910179157245&rtpof=true&sd=true

Выводы:

Итогом работы стал калькулятор, который помогает людям без расчетов получать данные, подставляя метрики для изменения. Кроме того, для изменения ситуации, на основании полученных данных предлагается:

- сделать акцент на постоянных пользователях, создав для них выгодные условия;
- поработать с ТОП-ом фильмов;
- проанализировать имеющиеся фиксированные затраты, пересмотреть возможность рекламы в странах, с большой численностью, а также возможности привлечения новых пользователей из стран, приносящих наибольшее количество прибыли.


Проект 3: **Когортный анализ онлайн-кинотеатра с помощью SQL**

Что нужно было сделать:

- выбрать фильмы и сериалы с определенным списком критериев и найти сколько суммарно они длятся;
- найти долю фильмов, попадающих под необходимые условия;
- построить распределение необходимых нам фильмов и сериалов;
- определить среднее количество голосов, на основании которых рассчитывается рейтинг у тайтлов.
- 
Как решала: 

Соединила необходимые для решения таблицы, прописала необходимые условия, вывела необходимый результат.

Ссылка на проект:

https://docs.google.com/document/d/1elOzxb-Y2msmb3kQKSPD80E9y2xpnSeL/edit?usp=sharing&ouid=118221966910179157245&rtpof=true&sd=true


Проект 4: **Моделирование изменения балансов студентов**

Что нужно было сделать:

Смоделировать изменение балансов студентов, для этого определить: 

- сколько всего уроков было на балансе всех учеников за каждый календарный день;
- как это количество менялось под влиянием транзакций и уроков;
- создать таблицу, где будут балансы каждого студента за каждый день.

Как решала: 

- узнала, когда была первая транзакция для каждого студента;
- собрала таблицу с датами за каждый календарный день необходимого нам года;
- узнала, за какие даты имеет смысл собирать баланс для каждого студента;
- нашла все изменения балансов, связанные с успешными транзакциями и  баланс студентов, который сформирован только транзакциями;
- нашла изменения балансов из-за прохождения уроков;
- создала CTE для хранения кумулятивной суммы количества пройденных уроков и CTE с вычисленными балансами каждого студента;
- посмотрела, как менялось общее количество уроков на балансах студентов.

Ссылка на проект:

https://docs.google.com/document/d/1Bo68CKO7yaUOCCm8uX4VgOxamqIKfXGb/edit?usp=sharing&ouid=118221966910179157245&rtpof=true&sd=true

Выводы:

Полученная визуализация позволяет нам увидеть полную картину. Графики накопительных сумм пройденных уроков уходитят вниз - это помогает увидеть списания с баланса, общий баланс показывается "серединой" между списанием и накоплением уроков. Также график помогает нам увидеть информацию по каждой точке - в определенный денть мы можем видеть ситуацию по пройденным и купленным урокам.

Кроме в процессе работы возникают вопросы к дата-инженерам:
1) Почему у части оплат нет id транзакции?
2) Почему у части студентов получается отрицательный баланс?

# Контактная информация
Email: kulagina_ma@mail.ru
