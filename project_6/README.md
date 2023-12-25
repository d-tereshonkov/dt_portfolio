# <p style="text-align: center;">Проект по SQL: Сервис для чтения книг <img src="https://img.icons8.com/external-bearicons-gradient-bearicons/64/external-SQL-file-extension-bearicons-gradient-bearicons.png" alt="external-SQL-file-extension-bearicons-gradient-bearicons" alt="image" width="40" height="35"></p>

### Описание задачи SQL:
Коронавирус застал мир врасплох, изменив привычный порядок вещей. В свободное время жители городов больше не выходят на улицу, не посещают кафе и торговые центры. Зато стало больше времени для книг. Это заметили стартаперы — и бросились создавать приложения для тех, кто любит читать.

Ваша компания решила быть на волне и купила крупный сервис для чтения книг по подписке. Ваша первая задача как аналитика — проанализировать базу данных.
В ней — информация о книгах, издательствах, авторах, а также пользовательские обзоры книг. Эти данные помогут сформулировать ценностное предложение для нового продукта.

### Описание данных:
Таблица books - Содержит данные о книгах:
- book_id — идентификатор книги;
- author_id — идентификатор автора;
- title — название книги;
- num_pages — количество страниц;
- publication_date — дата публикации книги;
- publisher_id — идентификатор издателя.

Таблица authors - Содержит данные об авторах:
- author_id — идентификатор автора;
- author — имя автора.

Таблица publishers - Содержит данные об издательствах:
- publisher_id — идентификатор издательства;
- publisher — название издательства.

Таблица ratings - Содержит данные о пользовательских оценках книг:
- rating_id — идентификатор оценки;
- book_id — идентификатор книги;
- username — имя пользователя, оставившего оценку;
- rating — оценка книги.

Таблица reviews - Содержит данные о пользовательских обзорах на книги:
- review_id — идентификатор обзора;
- book_id — идентификатор книги;
- username — имя пользователя, написавшего обзор;
- text — текст обзора.

**ER-диаграмма:**
- Структура данных БД

![ER-диаграмма](https://2.downloader.disk.yandex.ru/preview/f18a76e943e2a5034b764c67d71438ed5dd9d53a0dee46535314c34e89154222/inf/AJISjF4h-BPUuZeyyyQZsDYA0hPpw8437gQdx0o8XGbiT5GuN_HjXhr7xaLd_PbhdU6GUWwiRbfDd1J6kRtp8Q%3D%3D?uid=375844755&filename=ER-dia.jpg&disposition=inline&hash=&limit=0&content_type=image%2Fjpeg&owner_uid=375844755&tknv=v2&size=910x942](https://disk.yandex.ru/i/hL4Vyf9ceS-EEw)https://disk.yandex.ru/i/hL4Vyf9ceS-EEw)

