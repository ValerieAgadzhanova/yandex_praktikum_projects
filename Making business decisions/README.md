<img src="ab-testing.png" width=200 align="right"/>

# Описание проекта - Проверка гипотез по увеличению выручки в интернет-магазине
Проведена приоритизация гипотез по фреймворкам ICE и RICE. Затем провел анализ результатов A/B-теста, построил графики кумулятивной выручки, среднего чека, конверсии по группам, а затем посчитал статистическую значимость различий конверсий и средних чеков по сырым и очищенным данным.

## Используемые технологии
<div align="left">
<a href="https://www.python.org" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"/></a>
<a href="https://pandas.pydata.org" target="_blank"><img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Seaborn-047DA3?style=for-the-badge&logo=Codeforces&logoColor=white"/>
</a>
<a href="https://matplotlib.org/" target="_blank"><img src="https://img.shields.io/badge/Matplotlib-19A974?style=for-the-badge&logo=Codeforces&logoColor=white"/>
</a>
<a href="https://jupyter.org" target="_blank"><img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white"/>
</a>
</div> 

## Задача

- Примените фреймворк ICE для приоритизации гипотез. 
- Примените фреймворк RICE для приоритизации гипотез.
- Произвести оценку результатов A/B-тестирования различными методами

## Данные

Файл hypothesis.csv
- Hypothesis — краткое описание гипотезы;
- Reach — охват пользователей по 10-балльной шкале;
- Impact — влияние на пользователей по 10-балльной шкале;
- Confidence — уверенность в гипотезе по 10-балльной шкале;
- Efforts — затраты ресурсов на проверку гипотезы по 10-балльной шкале. Чем больше значение Efforts, тем дороже проверка гипотезы.
- 
Файл orders.csv
- transactionId — идентификатор заказа;
- visitorId — идентификатор пользователя, совершившего заказ;
- date — дата, когда был совершён заказ;
- revenue — выручка заказа;
- group — группа A/B-теста, в которую попал заказ.
- 
Файл visitors.csv
- date — дата;
- group — группа A/B-теста;
- visitors — количество пользователей в указанную дату в указанной группе A/B-теста
