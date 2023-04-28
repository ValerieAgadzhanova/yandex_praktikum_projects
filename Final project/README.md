<img src="app.png" width=200 align="right"/>

# Описание проекта - Выпускной проект. Анализ поведения пользователей в мобильном приложении

Финальный проект включает в себя работу над проектом, дашборд, задачи по A/B-тестированию и SQL.
Цель — проверить бóльшую часть навыков, которые были приобретены во время курса.

Задачи:
- Декомпозиция задания
- Исследовательский анализ данных
- [Дашборд](https://public.tableau.com/app/profile/valerieagadzhanova/viz/FinalProject_16732932562570/Dashboard)
- [Презентация](https://github.com/ValerieAgadzhanova/yandex_praktikum_projects/blob/115784ba73e0b4776cb7d9707217189deedb0c8d/Final%20project/%D0%9D%D0%B5%D0%BD%D1%83%D0%B6%D0%BD%D1%8B%D0%B5%20%D0%B2%D0%B5%D1%89%D0%B8.pdf)
- А/В-тестирование
- Проект по SQL

## Используемые технологии
<div align="left">
<a href="https://www.python.org" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"/></a>
<a href="https://pandas.pydata.org" target="_blank"><img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
</a>
<a href="https://matplotlib.org/" target="_blank"><img src="https://img.shields.io/badge/Matplotlib-19A974?style=for-the-badge&logo=Codeforces&logoColor=white"/>
</a>
<a href="https://scipy.org/" target="_blank"><img src="https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=SciPy&logoColor=white"/>
</a>
<a href="https://www.postgresql.org" target="_blank"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=PostgreSQL&logoColor=white"/></a>
<a href="https://plotly.com/python" target="_blank"><img src="https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=Plotly&logoColor=white"/>
</a>
<a href="https://jupyter.org" target="_blank"><img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white"/>
</a>
</div> 

# 1. Анализ поведения пользователей в мобильном приложении
Проанализировать поведение пользователей в приложении "Ненужные вещи". Определить типичные сценарии использования приложения и сегментировать пользователей для дальнейшего улучшения функционала. Проверить гипотезы.

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

# 2. А/B-тестирование
Провести оценку результатов A/B-теста. Оценить корректность проведения теста. Проанализировать результаты теста.

## Данные

ab_project_marketing_events.csv — календарь маркетинговых событий на 2020 год: 
- name — название маркетингового события;
- regions — регионы, в которых будет проводиться рекламная кампания;
- start_dt — дата начала кампании;
- finish_dt — дата завершения кампании.

final_ab_new_users.csv — все пользователи, зарегистрировавшиеся в интернет-магазине в период с 7 по 21 декабря 2020 года:
- user_id — идентификатор пользователя;
- first_date — дата регистрации;
- region — регион пользователя;
- device — устройство, с которого происходила регистрация.

final_ab_events.csv — все события новых пользователей в период с 7 декабря 2020 по 4 января 2021 года:
- user_id — идентификатор пользователя;
- event_dt — дата и время события;
- event_name — тип события;
- details — дополнительные данные о событии. Например, для покупок, purchase, в этом поле хранится стоимость покупки в долларах.

final_ab_participants.csv — таблица участников тестов:
- user_id — идентификатор пользователя;
- ab_test — название теста;
- group — группа пользователя.

# 3. Анализ данных сервиса для чтения книг (SQL)
Проанализировать базу данных, для формирования ценностного предложение для нового продукта.

## Данные
Таблица books
- book_id — идентификатор книги;
- author_id — идентификатор автора;
- title — название книги;
- num_pages — количество страниц;
- publication_date — дата публикации книги;
- publisher_id — идентификатор издателя.

Таблица authors
- author_id — идентификатор автора;
- author — имя автора.

Таблица publishers
- publisher_id — идентификатор издательства;
- publisher — название издательства;

Таблица ratings
- rating_id — идентификатор оценки;
- book_id — идентификатор книги;
- username — имя пользователя, оставившего оценку;
- rating — оценка книги.

Таблица reviews
- review_id — идентификатор обзора;
- book_id — идентификатор книги;
- username — имя пользователя, написавшего обзор;
- text — текст обзора.
