# <p style="text-align: center;">Анализ поведения пользователей в мобильном приложении <img src="https://img.icons8.com/color/48/member-skin-type-7.png" alt="image" width="40" height="35">
</p>

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
  - Одни пользователи совершают действия tips_show и tips_click , другие — только tips_show . Проверьте гипотезу: конверсия в просмотры контактов различается у этих двух групп.
  - Сформулируйте собственную статистическую гипотезу. Дополните её нулевой и альтернативной гипотезами. Проверьте гипотезу с помощью статистического теста.

**Рекомендации:**
- 65% пользователей видит рекомендованные объявления, но лишь 7% доходит до клика по нему, это говорит о неэффективности системы рекомендаций, чтобы повысить процент кликов по рекоментательному объявлению можно сделайть рекомендации более персонализированными, учитывая предпочтения и историю действий каждого пользователя. Тем самым повысим интерес пользователя, чем ближе по интересам рекомендации к конкретному пользователю, вероятность клика по объявлению больше. Также нужно проверить технические особенности(медленная ли прогрузка), визуальное оформление и размещение в рамках интерфейса.
- Низкий процент доходящих пользователей связанные с поиском по приложению до целевого действия - 19%, возможно связан с тем, что пользователи используя функционал поиска, находят не то, что им нужно. Программистам нужно поправить функционал фильтров поиска и сделать его более интуитивней.

- Конверсия в целевое действие - просмотр контактов: 23% очень маленькая, 77% пользователей не доходит до просмотра контакта, нужно повысить конверсию в просмотр контакта, путем упрощения процесса просмотра контактов, сделать его более простым, добавить обучающие элементы.

- Всего 351 пользователь использует функцию 'добавить объявление в избранное', что-бы привлечь больше пользователей к использованию данного функционала можно предлагать добавить объявление в избранное после просмотра или взаимодействия с ним.

- Конверсия пользователей открывших карту объявления в просмотр контактов низкая, чтобы ее повысить нужно убедиться, что на карте объявления доступна полная и релевантная информация о товаре или услуге, добавить привлекательные фотографии и видео товара, чтобы пользователи могли получить максимум информации.

**Презентация** - https://disk.yandex.com.am/i/dTJACOl2Y5JD7w

**Дашборд** - https://public.tableau.com/views/-_16956667328280/sheet2?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link
