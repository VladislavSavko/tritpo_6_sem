# TRiTPO

# Требования к проекту
---
# Содержание
1 [Введение](#intro)

1.1 [Название продукта](#product_name)
1.2 [Назначение документа](#appointment)  
1.3 [Бизнес-требования](#business_requirements)  
1.3.1 [Исходные данные](#initial_data)  
1.3.2 [Возможности бизнеса](#business_opportunities)  
1.3.3 [Границы проекта](#project_boundary)  
1.4 [Аналоги](#analogues)  
2 [Требования пользователя](#user_requirements)  
2.1 [Программные интерфейсы](#software_interfaces)  
2.2 [Интерфейс пользователя](#user_interface)  
2.3 [Характеристики пользователей](#user_specifications)  
2.3.1 [Классы пользователей](#user_classes)  
2.3.2 [Аудитория приложения](#application_audience)  
2.3.2.1 [Целевая аудитория](#target_audience)  
2.3.2.1 [Побочная аудитория](#collateral_audience)  
2.4 [Предположения и зависимости](#assumptions_and_dependencies)  
3 [Системные требования](#system_requirements)  
3.1 [Функциональные требования](#functional_requirements)  
3.1.1 [Основные функции](#main_functions)  
3.1.1.1 [Вход пользователя на сайт](#user_login_to_the_application)  
3.1.1.2 [Настройка профиля зарегистрированного пользователя](#setting_up_the_profile_of_the_active_user)    
3.1.1.3 [Просмотр информации об отдельном товаре](#view_information_about_an_individual_item)  
3.1.1.4 [Выход зарегистрированного пользователя из учётной записи](#active_user_change)  
3.1.1.5 [Регистрация нового пользователя после входа на сайт](#add_new_user)
3.1.1.6 [Просмотр информации обо всех товарах](#watch_items)
3.1.2 [Ограничения и исключения](#restrictions_and_exclusions)  
3.2 [Нефункциональные требования](#non-functional_requirements)  
3.2.1 [Атрибуты качества](#quality_attributes)  
3.2.1.1 [Требования к удобству использования](#requirements_for_ease_of_use)  
3.2.1.2 [Требования к безопасности](#security_requirements)  
3.2.2 [Внешние интерфейсы](#external_interfaces)  
3.2.3 [Ограничения](#restrictions)  
---


# 1 Введение
<a name="intro"/>

## 1.1 Название продукта
<a name="product_name"/>
PhoneShop

## 1.2 Назначение документа
<a name="appointment"/>
В этом документе описаны функциональные и нефункциональные требования к интернет-магазину PhoneShop.
Этот документ предназначен для команды, которая будет реализовывать и проверять корректность работы веб-сервиса.

## 1.3 Бизнес-требования
<a name="business_requirements"/>

### 1.3.1 Исходные данные
<a name="initial_data"/>
Шоппинг является одним из самых популярных видов досуга. Около 10 лет назад основными местами шоппинга для людей
любых возрастных категорий были торговые центры и специализированные площадки. Однако, не всегда имеется время для изучения всего ассортимента продукции интересуемого бренда, или, может не быть возможности посетить нужное место для шоппинга. С развитием технологий онлайн-магазинов люди получили возможность персонализировать свои интересы, выбирать нужные продукты онлайн, что означает трату меньшего времени, и просматривать ассортимент продукции любых брендов в Сети
В связи с этим появляется множество интернет-магазинов, позволяющих использовать технологии просмотра и подборки продуктов онлайн.

### 1.3.2 Возможности бизнеса
<a name="business_opportunities"/>
Многие люди желают иметь доступ к онлайн-магазину, позволяющий просматривать продукцию любых брендов онлайн, подбирать продукты для пользователя, основываясь на его предпочтениях и оценках. Подобная возможность позволит им тратить меньше времени на поиск необходимой информации и использовать онлайн-магазин в удобное время, не тратя лишнее время на поход по магазинам. Интерфейс, спроектированный с учётом всех особенностей похожих технологий, и дополнение онлайн-магазина подробной инструкцией позволят увеличить количество людей, использующих данный сервис.

### 1.3.3 Границы проекта
<a name="project_boundary"/>
Онлайн-магазин "PhoneShop" позволит зарегистрированным пользователям просматривать продукцию любых брендов и года выпуска онлайн, заказывать продукты с доставкой, просматривать историю цен на продукты.
Незарегистрированным пользователям будут доступны только:просмотр всей продукции и информации о конкретном продукте

## 1.4 Аналоги
<a name="analogues"/>
"5 элемент" — крупнейшая сеть электроники и бытовой техники в РБ. С 2012 года также доступен онлайн-магазин с несколькими тысячами товаров, в том числе эксклюзивных. Онлайн-магазин позволяет просматривать товары и получать подборки, основываясь на предпочтениях пользователя.

"21vek.by" — веб-сайт для просмотра и покупки бытовых товаров и электроники. По состоянию на январь 2021 года, на сайте доступно более чем 2 млн товаров. Сервис позволяет получать любые сведения о товарах и изучать оценки и отзывы пользователей.

"Электросила"  — одна из крупнейших сетей электроники и бытовой техники в РБ и РФ. С 2011 года доступен веб-сайт, позволяющий просматривать товары и получать доступ к оценкам и рецензиям, а также заказывать доставку необходимых товаров практически на любой адрес.

### 1.4.1 Отличия от аналогов
В отличие от "5 элемента" и "Электросилы" онлайн-магазин PhoneShop не позволяет заказывать товары на большинство адресов;
Также, в отличие от "21vek.by", на сайте будет доступно сравнительно меньшее количество товаров.

# 2 Требования пользователя
<a name="user_requirements"/>

## 2.1 Программные интерфейсы
<a name="software_interfaces"/>
Язык программирования: Java
API: Java EE
Фреймворки: Lombok, Java Media Framework

## 2.2 Интерфейс пользователя
<a name="user_interface"/>

Окно входа в сервис.  
![Окно входа в сервис](https://github.com/VladislavSavko/TRiTPO-lab2/blob/main/mockups/%D0%9C%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D0%B2%D1%85%D0%BE%D0%B4%D0%B0%20%D0%B2%20%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5.png)

Главное окно сервиса.
![Главное окно сервиса](https://github.com/VladislavSavko/TRiTPO-lab2/blob/main/mockups/%D0%9D%D0%BE%D0%B2%D1%8B%D0%B9%20%D0%BC%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%B3%D0%BB%D0%B0%D0%B2%D0%BD%D0%BE%D0%B3%D0%BE%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F.png)
 
Окно регистрации нового пользователя.
![Окно регистрации нового пользователя](https://github.com/VladislavSavko/TRiTPO-lab2/blob/main/mockups/%D0%9D%D0%BE%D0%B2%D1%8B%D0%B9%20%D0%BC%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D1%80%D0%B5%D0%B3%D0%B8%D1%81%D1%82%D1%80%D0%B0%D1%86%D0%B8%D0%B8%20%D0%BD%D0%BE%D0%B2%D0%BE%D0%B3%D0%BE%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8F.png)

Главное окно сервиса после выбора фильма.
![Главное окно сервиса после выбора фильма](https://github.com/VladislavSavko/TRiTPO-lab2/blob/main/mockups/%D0%9D%D0%BE%D0%B2%D1%8B%D0%B9%20%D0%BC%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%B3%D0%BB%D0%B0%D0%B2%D0%BD%D0%BE%D0%B3%D0%BE%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D0%BF%D0%BE%D1%81%D0%BB%D0%B5%20%D0%B2%D1%8B%D0%B1%D0%BE%D1%80%D0%B0%20%D1%84%D0%B8%D0%BB%D1%8C%D0%BC%D0%B0.png)

Окно настройки профиля пользователя.
![Окно настройки профиля пользователя](https://github.com/VladislavSavko/TRiTPO-lab2/blob/main/mockups/%D0%9D%D0%BE%D0%B2%D1%8B%D0%B9%20%D0%BC%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B8%20%D0%BF%D1%80%D0%BE%D1%84%D0%B8%D0%BB%D1%8F%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8F.png)

Окно просмотра фильма онлайн.
![Окно просмотра фильма онлайн](https://github.com/VladislavSavko/TRiTPO-lab2/blob/main/mockups/%D0%9C%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D0%BF%D1%80%D0%BE%D1%81%D0%BC%D0%BE%D1%82%D1%80%D0%B0%20%D1%84%D0%B8%D0%BB%D1%8C%D0%BC%D0%BE%D0%B2.png)

## 2.3 Характеристики пользователей
<a name="user_specifications"/>

### 2.3.1 Классы пользователей
<a name="user_classes"/>
1)Зарегистрированные пользователи - пользователи, которые вошли на веб-сайт под своим именем (псевдонимом), желающие просматривать товары, отобранные согласно их предпочтениям. Имеют доступ к полному функционалу

### 2.3.2 Аудитория приложения
<a name="application_audience"/>

#### 2.3.2.1 Целевая аудитория
<a name="target_audience"/>

##### 2.3.2.1.1 Младшая возрастная категория
Люди младшей возрастной категории(6-18) лет, обладающие минимальной технической грамотностью:умением взаимодействовать с компьютером.

##### 2.3.2.1.2 Средняя возрастная категория
Люди средней возрастной категории(18-60) лет, обладающие минимальной технической грамотностью:умением взаимодействовать с компьютером.

#### 2.3.2.2 Побочная аудитория
<a name="collateral_audience"/>
Люди старшей возрастной аудитории, обладающие вышеперечисленными качествами

### 2.4 Предположения и зависимости
<a name="assumptions_and_dependencies"/>
1. Веб-сайт должен иметь возможность обрабатывать значительное количество запросов в секунду;
2. Допустимое время ответа сервера не должно превышать 2 секунды;
3. На сервисе ожидается большое количество пользователей;
4. Требуется хранить значительное количество информации о товарах.

# 3 Cистемные требования
<a name="system_requirements"/>

## 3.1 Функциональные требования
<a name="functional_requirements"/>

### 3.1.1 Основные функции
<a name="main_functions"/>

#### 3.1.1.1 Вход пользователя на сайт
<a name="user_login_to_the_application"/>
**Описание.** Пользователь имеет возможность использовать сайт без создания собственного профиля либо войдя в свою учётную запись.

| Функция | Требования | 
|:---|:---|
| Вход на сайт без создания собственного профиля | Сайт должен предоставить пользователю возможность войти на сервис анонимно |
| Регистрация нового пользователя | Сайт должен запросить у пользователя ввести имя для создания учётной записи. Пользователь должен либо ввести имя, либо отменить действие |
| *Пользователь с таким именем существует* | *Сайт должно известить пользователя об ошибке регистрации и запросить ввод псевдонима. Пользователь должен либо ввести псевдоним, либо отменить действие* |
| Вход зарегистрированного пользователя на сайт | Сайт должен предоставить пользователю список имён (псевдонимов) зарегестрированных пользователей. Пользователь должен либо выбрать из списка своё имя (псевдоним), либо отменить действие |

#### 3.1.1.2 Настройка профиля зарегистрированного пользователя
<a name="setting_up_the_profile_of_the_active_user"/>
**Описание.** Зарегистрированный пользователь имеет возможность редактировать свой профиль, с которого производится выборка товаров

| Функция | Требования | 
|:---|:---|
| Редактирование общей информации о пользователе | Сайт должен предоставить зарегистрированному пользователю поле для ввода общей информации о себе. Пользователь должен либо ввести информацию и подвердить действие, либо отменить его |
| Редактирование информации о любимых жанрах фильмов | Зарегистрированный пользователь имеет возможножность редактировать список любимых жанров фильмов |

#### 3.1.1.3 Просмотр информации об отдельном товаре
<a name="view_information_about_an_individual_item"/>
**Описание.** Зарегистрированный пользователь имеет возможность просматривать краткую и полную информацию о товаре

| Функция | Требования | 
|:---|:---|
| Просмотр предварительной(краткой) информации | Сайт должен предоставить пользователю возможность увидеть краткую информацию о товаре на главной странице |
| Просмотр полной информации | Сайт должен предоставить пользователю возможность увидеть полную информацию о товаре |
| *Товара не существует* | *Сайт должен известить пользователя об ошибке, запросить повторный ввод и показать другие товары. Пользователь должен либо ввести информацию заново, либо выбрать другой товар, либо отменить действие* |

#### 3.1.1.4 Выход зарегистрированного пользователя из учетной записи
<a name="active_user_change"/>
**Описание.** Зарегистрированный пользователь имеет возможность выйти из своего профиля и продолжить работать с сайтом анонимно

**Требование.** Сайт должнен предоставить зарегистрированному пользователю возможность выйти из учётной записи с возвратом к окну входа на главную страницу.

#### 3.1.1.5 Регистрация нового пользователя после входа на сайт
<a name="add_new_user"/>
**Описание.** Пользователь имеет возможность зарегистрироваться в приложении.

**Требование.** Сайт должен предоставить пользователю возможность [зарегистрироваться в приложении]

#### 3.1.1.6 Просмотр информации обо всех товарах
<a name="watch_items"/>
**Описание.** Зарегистрированный пользователь имеет возможность просмотреть информацию обо всех товарах

**Требование.** Приложение должно предоставить пользователю возможность просмотра информации обо всех товарах

### 3.1.2 Ограничения и исключения
<a name="restrictions_and_exclusions"/>
1. Сайт работает только при наличии подключения к Интернету; 

## 3.2 Нефункциональные требования
<a name="non-functional_requirements"/>

### 3.2.1 Атрибуты качества
<a name="quality_attributes"/>

#### 3.2.1.1 Требования к удобству использования
<a name="requirements_for_ease_of_use"/>
1. Доступ к основным функциям приложения не более чем за две операции;
2. Все функциональные элементы пользовательского интерфейса имеют названия, описывающие действие, которое произойдет при выборе элемента;
3. Пошаговая инструкция использования основных функций приложения отображена в справке;
4. Обновление информации о товарах происходит каждые 30 минут в фоновом режиме.
5. Понятный графический интерфейс

#### 3.2.1.2 Требования к безопасности
<a name="security_requirements"/>
Сайт предоставляет возможность просмотра и редактирования профиля только активного пользователя.
Сайт гарантирует безопасность личных данных пользователей.

### 3.2.2 Внешние интерфейсы
<a name="external_interfaces"/>
Страницы сайта удобны для использования пользователями с плохим зрением:
  * размер шрифта не менее 14пт;
  * функциональные элементы контрастны фону станицы.

### 3.2.3 Ограничения
<a name="restrictions"/>
1. Приложение реализовано на платформе Java Servlet API
2. Профиль пользователя хранится в файле с расширением XML, название файла совпадает с именем (псевдонимом);
3. Информация о товарах хранится в базе данных MySQL.
4. Сайт не работает при отсутствии подключения к Интернету;
5. Сайти не обрабатывает данные товаров, недоступных в момент запроса;
6. Скорость работы сайта зависит от скорости подключения пользователя.
