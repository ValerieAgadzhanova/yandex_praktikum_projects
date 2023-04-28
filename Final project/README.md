<img src="app.png" width=200 align="right"/>

# Описание проекта - Выпускной проект. Анализ поведения пользователей в мобильном приложении

Финальный проект включает в себя работу над проектом, дашборд, задачи по A/B-тестированию и SQL.
Цель — проверить бóльшую часть навыков, которые были приобретены во время курса.

## Используемые технологии
<div align="left">
<a href="https://www.python.org" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"/></a>
<a href="https://pandas.pydata.org" target="_blank"><img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
</a>
<a href=# target="_blank"><img src="https://img.shields.io/badge/Seaborn-047DA3?style=for-the-badge&logo=Codeforces&logoColor=white"/>
</a>
<a href="https://matplotlib.org/" target="_blank"><img src="https://img.shields.io/badge/Matplotlib-19A974?style=for-the-badge&logo=Codeforces&logoColor=white"/>
</a>
<a href="https://plotly.com/python" target="_blank"><img src="https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=Plotly&logoColor=white"/>
</a>
<a href="https://jupyter.org" target="_blank"><img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white"/>
</a>
</div> 

## Задача

- Декомпозиция задачи
- Исследовательский анализ
- Создание дашборда
- Подготовка презентации
- Проект по А/Б-тестированию
- Проект по SQL

## Данные
В датасете содержатся данные пользователей, впервые совершивших действия в приложении после 7 октября 2019 года.

Колонки в mobile_sources.csv:
- userId — идентификатор пользователя,
- source — источник, с которого пользователь установил приложение.

Колонки в mobile_dataset.csv: 
- event.time — время совершения,
- user.id — идентификатор пользователя,
- event.name — действие пользователя.
- 
Виды действий:
- advert_open — открыл карточки объявления,
- photos_show — просмотрел фотографий в объявлении,
- tips_show — увидел рекомендованные объявления,
- tips_click — кликнул по рекомендованному объявлению,
- contacts_show и show_contacts — посмотрел номер телефона,
- contacts_call — позвонил по номеру из объявления,
- map — открыл карту объявлений,
- search_1—search_7 — разные действия, связанные с поиском по сайту,
- favorites_add — добавил объявление в избранное.
