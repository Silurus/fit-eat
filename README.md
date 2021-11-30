# Eat-Fit - сервис доставки здоровой еды

## Предметная область
Сервис доставки здоровой еды через мобильное приложение.

**Целевая аудитория**: люди в возрасте от 20 до 50 лет, следящие за своим питанием и желающие разнообразить свой рацион, не выходя за рамки диеты.

## Схема БД

БД ориентирована на оформление заказов из мобильного приложения, где клиенты могут отслеживать статус заказа и ориентировочное время доставки.

По каждому выполненному заказу клиенту предлагается оценить заказ и работу курьера.
На основе этих данных курьерам выставляется средний рейтинг и дорабатывается рецептура блюд.

![image](https://user-images.githubusercontent.com/19695435/144134960-13b9db6e-be44-4adb-8147-8b06c95c0a37.png)


### Описание таблиц

- **Customer** - таблица с данными о клиентах
- **Address** - таблица с адресами доставки заказов. Также используется для хранения адресов клиентов по-умолчанию
- **Order** - таблица с данными о заказах
- **OrderQueue** - таблица-очередь заказов. Здесь хранится статус заказа, ожидаемое время доставки, а также назначенный на заказ курьер
- **Courier** - таблица с курьерами. У каждого курьера есть средний рейтинг, который складывается из рейтинга всех доставленных заказов
- **Payment** - таблица с данными об оплате заказа
- **OrderList** - таблица с данными о составе заказа (блюдо, количество)
- **Meal** - таблица с данными о блюдах. Здесь хранится описание, размер порции, состав, КБЖУ
- **OrderFeedback** - таблица с отзывами пользователей о заказах. Используется для формирования рейтинга курьеров.
