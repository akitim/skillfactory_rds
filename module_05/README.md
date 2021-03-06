# Проект 5. Компьютер говорит «Нет»
## Юнит 5. Основные алгоритмы машинного обучения. Часть I   
### skillfactory_rds

![https://colab.research.google.com/assets/colab-badge.svg](https://colab.research.google.com/assets/colab-badge.svg)

## Оглавление  
[1. Описание модуля](https://github.com/akitim/skillfactory_rds/blob/main/module_05/README.md#Описание-модуля)<br>
[2. Информация о данных](https://github.com/akitim/skillfactory_rds/blob/main/module_05/README.md#Информация-о-данных)<br>
[3. Работа над проектом](https://github.com/akitim/skillfactory_rds/blob/main/module_05/README.md#Работа-над-проектом)<br>
[4. Результат](https://github.com/akitim/skillfactory_rds/blob/main/module_05/README.md#Результат)

### Описание модуля  

***Чем мы будем заниматься?***  
- Напишем скоринговую модель предсказания дефолта клиентов банка.  
- Поучаствуем в командном хакатоне (на этот раз мы приготовили для вас неожиданный формат).  
:arrow_up:[к оглавлению](https://github.com/akitim/skillfactory_rds/blob/main/module_05/README.md#Оглавление)

**Условия соревнования:**  
Тестовая выборка представлена в LeaderBoard целиком.  
Поэтому лучшие и победные решения буду проверяться на их "адекватность" (чтоб не было подгонки под тестовую выборку).  
Разрешено использовать любые ML алгоритмы и библиотеки (кроме DL).  
Делаем реальный ML продукт, который потом сможет нормально работать на новых данных.  

**Метрика качества**
Результаты оцениваются по метрике F1
:arrow_up:[к оглавлению](https://github.com/akitim/skillfactory_rds/blob/main/module_05/README.md#Оглавление)

### Информация о данных
*Определение.* Кредитная история — это карточка заёмщика, в которую записываются все операции с кредитами: какой банк выдавал, сколько есть долгов и вовремя ли платит гражданин. Основание: Федеральный закон «О кредитных историях».  

Датасет содержит информацию о заемщиках, которые уже брали кредиты (повторных клиентов).  
Вам предоставлена информация из анкетных данных заемщиков и факт наличия дефолта. 

Описание столбцов датасета:  
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
:arrow_up:[к оглавлению](https://github.com/akitim/skillfactory_rds/blob/main/module_05/README.md#Оглавление)

### Работа над проектом  
- Работа над проектом велась мной самостоятельно без команды.<br>
:arrow_up:[к оглавлению](https://github.com/akitim/skillfactory_rds/blob/main/module_05/README.md#Оглавление)

### Результат  
score А1 = 0.33484, 14 место на в LeaderBoard на kaggle.
Оценка командой курса - __ баллов из 21: 
- Качество кода. Стандарты кода и написания функций/классов (если есть) (соблюдение стандартов оформления) — из 3 баллов.
- Качество разведывательного анализа данных (визуализация, очистка данных, работа с выбросами) — 3 баллов.
- Проектирование признаков (выбор признаков, генерация новых признаков) — 3 баллов.
- Работа с метрикой, правильность выбора метрики, интерпретация результатов полученных моделей — 3 баллов.
- Умение решать задачи классификации — 3 баллов.
- *Настройка гиперпараметров - из 3 баллов
- *Умение работать в команде - из 3 баллов

:arrow_up:[к оглавлению](https://github.com/akitim/skillfactory_rds/blob/main/module_05/README.md#Оглавление)
