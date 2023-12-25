# <p style="text-align: center;">Анализ поведения пользователей в мобильном приложении </p><img src="https://img.icons8.com/color/48/member-skin-type-7.png" alt="image" width="40" height="35">

**Описание данных:**

Датасет содержит данные о событиях, совершенных в мобильном приложении
"Ненужные вещи". В нем пользователи продают свои ненужные вещи, размещая их на доске объявлений.
В датасете содержатся данные пользователей, впервые совершивших действия в
приложении после 7 октября 2019 года.

Колонки в /datasets/mobile_sources.csv:

- userId — идентификатор пользователя,
- source — источник, с которого пользователь установил приложение.
    
Колонки в /datasets/mobile_dataset.csv:

- event.time — время совершения,
- user.id — идентификатор пользователя,
- event.name — действие пользователя.
    
    Виды действий:
        - advert_open — открыл карточки объявления,
        - photos_show — просмотрел фотографий в объявлении,
        - tips_show — увидел рекомендованные объявления,
        - tips_click — кликнул по рекомендованному объявлению,
        - contacts_show и show_contacts — посмотрел номер телефона,
        - contacts_call — позвонил по номеру из объявления,
        - map — открыл карту объявлений,
        - search_1 — search_7 — разные действия, связанные с поиском по сайту,
        - favorites_add — добавил объявление в избранное.
        
По итогам исследования подготовим презентацию.

Моя задача, как аналитика на испытательном сроке в компании мобильного приложения "Ненужные вещи" выполнить анализ поведения пользователей. 
Основная цель - определить как можно улучшить приложение с точки зрения пользовательского опыта для увеличения вовлеченности пользователей в приложении до целевого действия - просмотр контактов.

**Задачи исследования:**
1. Проанализировать связь целевого события — просмотра контактов — и других действий пользователей.
2. Оценить, какие действия чаще совершают те пользователи, которые просматривают контакты.

**Этапы исследования:**
- Проведите исследовательский анализ данных
- Проанализируйте влияние событий на совершение целевого события
- Проверьте статистические гипотезы:
    1. Одни пользователи совершают действия tips_show и tips_click , другие — только tips_show . Проверьте гипотезу: конверсия в просмотры контактов различается у этих двух групп.
    2. Сформулируйте собственную статистическую гипотезу. Дополните её нулевой и альтернативной гипотезами. Проверьте гипотезу с помощью статистического теста.