# Marina
# Обо мне
Привет! Меня зовут Марина, я начинающий аналитик данных. В этом репозитории вы можете найти некоторые из моих проектов, выполненных во время обучения и практики.

# Навыки и технологии
Инструменты анализа данных: SQL, Excel

Системы управления базами данных: PostgreSQL

# Проекты
Проект 1: Калькулятор юнит-экономики онлайн-школы

Что нужно было сделать:

1. Рассчитать на какую сумму мы могли бы увеличить расходы на основных сотрудников в апреле 2021 года при условии, что маржинальность в этом месяце не должна упасть ниже 11%?
2. Рассчитать какой станет маржинальность за март 2021, если доля бесплатных уроков в нем упадет на 10 процентных пунктов*?
3. Рассчитать насколько увеличится LTR и маржинальность апреля 2021 года, если средний Retention будет на 2 процентных пункта выше?

Как решала: 
1. Представила, что маржинальность апреля 2021 года равна 11%, при этом Выручка, ЗП учителей и CAC не изменились. Затем рассчитала ФОТ и то, на сколько он больше, чем был по факту в апреле 2021 года.
2. Посчитала доли уроков разной цены в марте 2021 года, рассчитала долю бесплатных уроков, представила, что было бы, если бы их было на 10 процентных пунктов меньше, а уроков за 1200 рублей на то же количество уроков больше, рассчитала выручку. Подставила в март получившуюся рассчётную выручку. Рассчитала маржинальность.
3. Увеличила Retention на 2 процентных пункта и пересчитала Lifetime, пересчитала LTRю Для апреля 2021 год пересчитала долю расходов на привлечение %CAC при том, что сам CAC в абсолютном выражении останется прежним - на уровне 13140,72 рублей. Получила новую маржинальность.

Ссылка на проект (прикладываю скриншоты результатов работы,т. к. данные конфеденциальны):

https://drive.google.com/file/d/1R2_nui_DEwgdiEiKBg6X0ejz-NHtA65N/view?usp=sharing

https://drive.google.com/file/d/1s9bbG_oUS7u18E5-M6xym3vMIfPZvB_1/view?usp=sharing

https://drive.google.com/file/d/1s-0bliuXMVmPb4H1-m94E_9In0Ud98-X/view?usp=sharing

Выводы:

На основании данных, полученных от работодателя были выполнены перерасчеты, в результате которых получили маржинальность проекта при различных условиях.

Проект 2: Калькулятор юнит-экономики онлайн-кинотеатра

Что нужно было сделать:
1. Необходимо посчитать юнит-экономику продукта
2. Предложить сценарий по настройке параметров для выхода на 25-процентную маржинальность
3. Собрать наглядную визуализацию, где будет показано, кто, где и в каком объеме смотрит фильмы платформе

Как решала: 
1. Рассчитала необходимые для дальнейшей работы метрики (количество подписок в каждый месяц, просмотров в каждый месяц, уникальных просматривающих пользователей в каждый месяца, дата первого просмотра для каждого юзера, количество первых просмотров для пользователя в каждый месяц, среднее количество просмотров на одного юзера в каждом месяце)
2. На основании этих данных рассчитала:
1) Количество повторных оплат в каждом месяце
2) Retention для каждого месяца
3) Среднее геометрическое Retention    
4) Lifetime       
5) LTR 
6) CAC    
7) Маржинальность
3. Подогнала параметры таким образом, чтобы маржинальность была +25%, построила необходимые графики.

Ссылка на проект:

https://docs.google.com/presentation/d/1U80E1uWVe68SOl8wRHZ9ToOcHP95RFd5/edit?usp=sharing&ouid=118221966910179157245&rtpof=true&sd=true

Выводы:

1. На основе проанализированных данных предлагается сделать акцент на постоянных пользователях, создав для них выгодные условия и возможность заморозки, возможно, индивидуальные предложения для определенного числа пользователей, уменьшить процент скидок и тем самым поднять средний чек.
2. В дальнейшем предлагается поработать с ТОП-ом фильмов, увеличив количество из переводов, а также, пересмотреть затраты на фильмы, которые просматриваются меньше всего, отказавшись от них в пользу новых, список которых мы могли бы определить с помощью анализа интернет-просмотров и рейтинга фильмов.
3. Предполагается проанализировать имеющиеся фиксированные затраты, пересмотреть возможность рекламы в странах, с большой численностью, а также возможности привлечения новых пользователей из стран, приносящих наибольшее количество прибыли.


Проект 3: Когортный анализ онлайн-кинотеатра с помощью SQL

Что нужно было сделать:
1. Выбрать жанр Animation. Ограничьтесь только фильмами и сериалами, которые были выпущены позже 1990 года и у которых рейтинг больше 8. Найти сколько суммарно они длятся (в часах). Получить таблицу-результат: суммарную длительность (одно значение).
2. Найти у какой доли фильмов/сериалов нет рейтинга? Взять только произведения, выпущенные позже 1950 года и длящиеся дольше 60 минут. Ответ дать в целых процентах. Получить таблицу-результат: долю (одно значение).
3. Построить распределение фильмов/сериалов с пометкой «для взрослых» по рейтингу. Создать интервалы для бинирования (интервалирования) рейтинга с шагом 1.5 и посмотреть количество позиций в каждом бине рейтинга. Не включать позиции без рейтинга. Брать только позиции, снятые позже 1975 года. Отранжировать результат по возрастанию бинов рейтинга.
4. Определить среднее количество голосов, на основании которых рассчитывается рейтинг у тайтлов. Интересуют те тайтлы, которые отсутствуют в таблице title_basics и средний рейтинг по которым больше 7.

Как решала: 
Соединила необходимые для решения таблицы, прописала необходимые условия, вывела необходимый результат.

Ссылка на проект:

https://docs.google.com/document/d/1elOzxb-Y2msmb3kQKSPD80E9y2xpnSeL/edit?usp=sharing&ouid=118221966910179157245&rtpof=true&sd=true


Проект 4: Построение витрины для модели машинного обучения в банке

Что нужно было сделать: задача №1.

Как решала(-а): краткое описание решения (автореферат)

Ссылка на проект (ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)

Выводы:

Итог №1
Итог №2

Проект 5: Моделирование изменения балансов студентов

Что нужно было сделать:

Смоделировать изменение балансов студентов. Баланс — это количество уроков, которое есть у каждого студента. Чтобы проверить, всё ли в порядке с нашими данными и составить список гипотез и вопросов, нам важно понимать: 
- Сколько всего уроков было на балансе **всех учеников** за каждый календарный день
- Как это количество менялось под влиянием транзакций (оплат, начислений, корректирующих списаний) и уроков (списаний с баланса по мере прохождения уроков)
Также нам нужно создать таблицу, где будут балансы **каждого студента** за каждый день.
В результате должен получиться запрос, который собирает данные о балансах студентов за каждый прожитый ими день.

Как решала: 
1. Узнала, когда была первая транзакция для каждого студента. Начиная с этой даты, мы будем собирать его баланс уроков. 
2. Собрала таблицу с датами за каждый календарный день 2016 года. Выбрала все даты из таблицы `classes`, **создадала CTE** `all_dates` с полем `dt`, где будут храниться уникальные даты (без времени) уроков. 
3. Узнала, за какие даты имеет смысл собирать баланс для каждого студента. Для этого объединила таблицы и создадим CTE `all_dates_by_user`, где будут храниться все даты жизни студента после того, как произошла его первая транзакция.  
4. Нашла все изменения балансов, связанные с успешными транзакциями. Выбрала все транзакции из таблицы `payments`, сгруппировала их по `user_id` и дате транзакции и нашла сумму по полю `classes`. 
**В результате** получила CTE `payments_by_dates` с полями: `user_id`, `payment_date`, `transaction_balance_change` (сколько уроков было начислено или списано в этот день). 
5. Нашла баланс студентов, который сформирован только транзакциями. Для этого объединила `all_dates_by_user` и `payments_by_dates` так, чтобы совпадали даты и `user_id`. Используя оконные выражения (функцию `sum`), чтобы найти кумулятивную сумму по полю `transaction_balance_change` для всех строк до текущей включительно с разбивкой по `user_id` и сортировкой по `dt`. 
**В результате** получила CTE `payments_by_dates_cumsum` с полями: `user_id`, `dt`, `transaction_balance_change` — `transaction_balance_change_cs` (кумулятивная сумма по `transaction_balance_change`). 
6. Нашла изменения балансов из-за прохождения уроков. Создала CTE `classes_by_dates`, посчитав в таблице `classes` количество уроков за каждый день для каждого ученика. Исключила вводные уроки и уроки со статусом, отличным от `success` и `failed_by_student`. 
**Получила результат** с такими полями: `user_id`, `class_date`, `classes` (количество пройденных в этот день уроков). Причем `classes` умножила на `-1`, чтобы отразить, что `-` — это списания с баланса.
7. По аналогии с уже проделанным шагом для оплат создала CTE для хранения кумулятивной суммы количества пройденных уроков.  Для этого объединила таблицы `all_dates_by_user` и `classes_by_dates` так, чтобы совпадали даты и `user_id`. Использовала оконные выражения (функцию `sum`), чтобы найти кумулятивную сумму по полю `classes` для всех строк до текущей включительно с разбивкой по `user_id` и сортировкой по `dt`. **В результате** получила CTE `classes_by_dates_dates_cumsum`с полями: `user_id`, `dt`, `classes` — `classes_cs`(кумулятивная сумма по `classes`). При подсчете кумулятивной суммы заменила пустые значения нулями.
8. Создала CTE `balances` ****с вычисленными балансами каждого студента. Для этого объединила таблицы `payments_by_dates_cumsum` ****и `classes_by_dates_dates_cumsum` так, чтобы совпадали даты и `user_id`.**Получила такие поля:** `user_id`, `dt`, `transaction_balance_change`, `transaction_balance_change_cs`, `classes`, `classes_cs`, `balance` (`classes_cs` + `transaction_balance_change_cs`).
9. Посмотрела, как менялось общее количество уроков на балансах студентов. Для этого просуммировала поля `transaction_balance_change`, `transaction_balance_change_cs`, `classes`, `classes_cs`, `balance` из CTE `balances` с группировкой и сортировкой по `dt`.

Ссылка на проект:

https://docs.google.com/document/d/1Bo68CKO7yaUOCCm8uX4VgOxamqIKfXGb/edit?usp=sharing&ouid=118221966910179157245&rtpof=true&sd=true

Выводы:

По результатам работы у дата-инженеров хочется уточнить:
1) Почему у части оплат нет id транзакции?
2) Почему у части студентов получается отрицательный баланс?

# Контактная информация
Email: kulagina_ma@mail.ru
