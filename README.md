# PROJECT-2. Анализ резюме из HeadHunter
Основной ноутбук - Project-2.ipynb

Данные , использованные в проекте, хранятся под управлением СУБД PostgreSQL. Для входа в базу использованы данные: 

    DBNAME = 'project_sql'
    USER = 'skillfactory'
    PASSWORD = 'cCkxxLVrDE8EbvjueeMedPKt'
    HOST = '84.201.134.129'
    PORT = 5432

## Оглавление  
[1. Описание проекта](https://github.com/balkhinag/Project_2/blob/main/README.md#%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)  
[2. Какой кейс решаем?](https://github.com/balkhinag/Project_1#%D0%BA%D0%B0%D0%BA%D0%BE%D0%B9-%D0%BA%D0%B5%D0%B9%D1%81-%D1%80%D0%B5%D1%88%D0%B0%D0%B5%D0%BC)  
[3. Краткая информация о данных](https://github.com/balkhinag/Project_1#%D0%BA%D1%80%D0%B0%D1%82%D0%BA%D0%B0%D1%8F-%D0%B8%D0%BD%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D1%8F-%D0%BE-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)  
[4. Этапы работы над проектом](https://github.com/balkhinag/Project_1#%D1%8D%D1%82%D0%B0%D0%BF%D1%8B-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B-%D0%BD%D0%B0%D0%B4-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%BC)  
[5. Результат](https://github.com/balkhinag/Project_1#%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82%D1%8B)    
[6. Выводы](https://github.com/balkhinag/Project_1#%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B) 

### Описание проекта   
Проблематика: необходимо создать модель машинного обучения, которая будет рекомендовать вакансии клиентам кадрового агентства, претендующим на позицию Data Scientist. Задача текущего проекта состоит в том, чтобы понять, что из себя представляют данные и насколько они соответствуют целям проекта

:arrow_up:[к оглавлению](_)


### Какой кейс решаем?    
Проводим анализ данных (Data Understanding), чтобы понять, что из себя представляют данные и насколько они соответствуют целям проекта

:arrow_up:[к оглавлению](.README.md#Оглавление)

### Краткая информация о данных
В нашем распоряжении 5 таблиц, которые находятся в схеме public базы данных project_sql:
- VACANCIES: Таблица хранит в себе данные по вакансиям
- AREAS: Таблица-справочник, которая хранит код города и его название
- EMPLOYERS: Таблица-справочник со списком работодателей
- INDUSTRIES: Таблица-справочник вариантов сфер деятельности работодателей
- EMPLOYERS_INDUSTRIES: Дополнительная таблица, которая существует для организации связи между работодателями и сферами их деятельности.Эта таблица нужна нам, поскольку у одного работодателя может быть несколько сфер деятельности (или работодатели могут вовсе не указать их). Для удобства анализа необходимо хранить запись по каждой сфере каждого работодателя в отдельной строке таблицы.
  
:arrow_up:[к оглавлению](.README.md#Оглавление)


### Этапы работы над проектом  
- знакомство с данными
- предварительный анализ данных
- детальный анализ вакансий
- анализ работодателей
- предметный анализ

Каждый этап состоит из блока практических заданий, которые выполнены в ноутбуке, и контрольных вопросов на обучающей платформе Skillfactory.ru

:arrow_up:[к оглавлению](.README.md#Оглавление)


### Результаты:  
По итогам проделанной работы мы получили следующий результат:
- Проовели детальный анализ вакансий, работодателей и требования работодателей к дата-сайентистам
- Выявили, что средняя заработная плата по всем вакансиям в представленных данных (71-110 тысяч) сильно превышает среднюю ЗП по России
- Выявили, что работодатели чаще всего ищут сотрудников с опытом работы от 1 до 3 лет - таких вакансий оказалось больше половины
- Проанализировали, сколько вакансий имеет отношение к данным
- Проанализировали, ключевые навыки, среднюю ЗП в зависимости от опыта для специалистов по Data Scince

:arrow_up:[к оглавлению](.README.md#Оглавление)


### Выводы:  
В результате проделанного проекта удалось испытать на себе основные этапы работы с данными на примере датасета о резюме соискателей

:arrow_up:[к оглавлению](.README.md#Оглавление)

