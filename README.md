# Что происходит с экологией в России и какова роль государства и НКО?
### Итоговый проект по Открытым данным

**Дата:** 24.03.25

**Автор:** Соловьева Анна

### Структура проекта
Проект состоит из двух частей:

1.**Работа с открытыми данными**
- Источник №1. [Росстат. Основные показатели охраны окружающей среды. 2023](https://docs.yandex.ru/docs/view?tm=1742671703&tld=ru&lang=ru&name=oxr_bul_2023.pdf&text=%D1%8D%D0%BA%D0%BE%D0%BB%D0%BE%D0%B3%D0%B8%D1%8F%20%D1%80%D0%BE%D1%81%D1%81%D0%B8%D1%8F%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D0%B5&url=https%3A%2F%2Frosstat.gov.ru%2Fstorage%2Fmediabank%2Foxr_bul_2023.pdf&lr=11499&mime=pdf&l10n=ru&sign=03ba52388791b96b6942021f812bb66c&keyno=0&nosw=1&serpParams=tm%3D1742671703%26tld%3Dru%26lang%3Dru%26name%3Doxr_bul_2023.pdf%26text%3D%25D1%258D%25D0%25BA%25D0%25BE%25D0%25BB%25D0%25BE%25D0%25B3%25D0%25B8%25D1%258F%2B%25D1%2580%25D0%25BE%25D1%2581%25D1%2581%25D0%25B8%25D1%258F%2B%25D0%25B4%25D0%25B0%25D0%25BD%25D0%25BD%25D1%258B%25D0%25B5%26url%3Dhttps%253A%2F%2Frosstat.gov.ru%2Fstorage%2Fmediabank%2Foxr_bul_2023.pdf%26lr%3D11499%26mime%3Dpdf%26l10n%3Dru%26sign%3D03ba52388791b96b6942021f812bb66c%26keyno%3D0%26nosw%3D1)
- Источник №2. [Росприроднадзор](https://rpn.gov.ru/open-service/analytic-data/statistic-reports/production-consumption-waste/)

На этом этапе был осуществлен поиск, отбор, концептуализация содержания данных, а также их объединение посредством Google Sheets (функция ВПР была применена для объединения данных за 2021, 2022 и 2023 годы по регионам). [Ссылка на таблицу](https://docs.google.com/spreadsheets/d/1t8Bz2qaLbntjJ4CYP2U4VqvACTvLFGN9KObSsbNMhC8/edit?usp=sharing)

Помимо этого, таблицы были преобразованы в машиночитаемый формат csv для дальнейшей работы в pandas.

В процессе анализа полученных данных были сделаны некоторые предположения о государственном недофинансировании обращения с отходами. Предположения были соотнесены с аналитическими источниками: 
- [Ведомости](https://www.vedomosti.ru/economics/articles/2019/10/17/814026-finansirovanie-reformi). 2019 год.
- [Finexpertiza](https://finexpertiza.ru/press-service/researches/2023/zakh-80-musora/). 2023 год.

2. **Парсинг данных о пользователях групп Вконтакте**
Сообщества экологической направленности (сбор и сортировка мусора, рециклинг, забота об окружающей среде), которые были выбраны для анализа профилей учатников:
- [Экологическое движение «РазДельный Сбор»](https://vk.com/rsbor)
- [Круг Жизни, Межрегиональный Центр, АНО](https://vk.com/vkrugorg)
- [Экоцентр Сборка](https://vk.com/ecosborka)
- [#МосЭко | #РосЭко](https://vk.com/moseco)
- [Экологическое движение «Мусора.Больше.Нет»](https://vk.com/musora_bolshe_net)
- [ЭкоСборная России](https://vk.com/ecosophy)

Отдельно я решила проанализировать самые крупные эко-сообщества вузов, которые занимаются продвижанием экологичного образа жизни в университетах НИУ ВШЭ, МГИМО и МГУ:
- [Дружина охраны природы МГУ](https://vk.com/dop_msu)
- [MGIMO Goes Green](https://vk.com/mgimogoesgreen)
- [Зелёная Вышка](https://vk.com/hsegreen)

После подключения к API Вконтакте и загрузке данных о пользователях, я провела преобразование данных и разведочный анализ.

- Преобразовала возраст пользователей, а затем проанализировала, очистила от выбросов и сравнила
- Выделила и составила топ университетов, в которых учились/учатся пользователи групп
- Перекодировала пол и проанализировала соотношение мужчин и женщин, состоящих в эко-группах

## Лицензия

Свободная лицензия - [CC 4.0](https://creativecommons.org/licenses/by/4.0/?region=international)

