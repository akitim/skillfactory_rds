# Проект 5. Компьютер говорит «Нет»
## Юнит 5. Основные алгоритмы машинного обучения. Часть I   
### skillfactory_rds  
![https://img.shields.io/badge/Python-3.7.4-blue](https://img.shields.io/badge/Python-3.8.x-blue)

## Оглавление  
[1. Описание модуля] 
[2. Информация о данных] 
[3. Работа над проектом]
[4. Результат]  

### Описание модуля  
В этом модуле вас ждёт путь от стажёра отдела аналитики регионального банка до… Будем считать, что почти до начальника отдела!  

***Чем мы будем заниматься?***  
- Напишем скоринговую модель предсказания дефолта клиентов банка.  
- Поучаствуем в командном хакатоне (на этот раз мы приготовили для вас неожиданный формат).  
:arrow_up:[к оглавлению]

**Условия соревнования:**  
Тестовая выборка представлена в LeaderBoard целиком.  
Поэтому лучшие и победные решения буду проверяться на их "адекватность" (чтоб не было подгонки под тестовую выборку).  
Разрешено использовать любые ML алгоритмы и библиотеки (кроме DL).  
Делаем реальный ML продукт, который потом сможет нормально работать на новых данных.  

**Метрика качества**
Результаты оцениваются по метрике F1
:arrow_up:[к оглавлению](https://github.com/alex-sokolov2011/skillfactory_rds/blob/master/module_4/README.md#Оглавление)

### Информация о данных
*Определение.* Кредитная история — это карточка заёмщика, в которую записываются все операции с кредитами: какой банк выдавал, сколько есть долгов и вовремя ли платит гражданин. Основание: Федеральный закон «О кредитных историях».  

Датасет содержит информацию о заемщиках, которые уже брали кредиты (повторных клиентов).  
Вам предоставлена информация из анкетных данных заемщиков и факт наличия дефолта.  
Описание полей датасета:  
- client_id	- идентификатор клиента  
- education	- уровень образования (ACD - academy - академическое, PGR - post-graduate - магистратура, GRD - graduate - бакалавриат, SCH - school - среднее)  
- sex	- пол заёмщика  
- age	- возраст заёмщика  
- car	- флаг наличия автомобиля  
- car_type	- флаг автомобиля-иномарки  
- decline_app_cnt	- количество отказанных прошлых заявок  
- good_work	- флаг наличия «хорошей» работы  
- bki_request_cnt	- количество запросов в БКИ  
- home_address	- категоризатор домашнего адреса  
- work_address	- категоризатор рабочего адреса  
- income	- доход заёмщика  
- foreign_passport	- наличие загранпаспорта  
- sna - связь заемщика с клиентами банка  
- first_time - давность наличия информации о заемщике  
- score_bki - скоринговый балл по данным из БКИ  
- region_rating - рейтинг региона  
- app_date - дата подачи заявки  
- default	- наличие дефолта  
:arrow_up:[к оглавлению]

### Работа над проектом  
- после того как мы определились, что выбранная метрика ROC_AUC не эффективно определяет качество алгоритма определения дефолтных клиентов (ошибка второго рода) мы сфокусировались на том чтобы не гнаться за лидербордом, а сделать рабочий продукт. Поэтому выбрали метрику ROC_PR и f1  
:arrow_up:[к оглавлению]

### Результат  
score ROC-AUC = 0.73650, 5 место на kaggle из 14 команд закрытого соревнования (Топ 36%).
Оценка командой курса - 97 баллов из 100: 
- Качество кода. Стандарты кода и написания функций/классов (если есть) (соблюдение стандартов оформления) — из 3 баллов.
- Качество разведывательного анализа данных (визуализация, очистка данных, работа с выбросами) — 3 баллов.
- Проектирование признаков (выбор признаков, генерация новых признаков) — 3 баллов.
- Работа с метрикой, правильность выбора метрики, интерпретация результатов полученных моделей — 3 баллов.
- Умение решать задачи классификации — 3 баллов.
- *Настройка гиперпараметров - из 3 баллов
- *Умение работать в команде - из 3 баллов

:arrow_up:[к оглавлению](https://github.com/alex-sokolov2011/skillfactory_rds/blob/master/module_4/README.md#Оглавление)
