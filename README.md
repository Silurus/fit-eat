# fit-eat

## Предметная область
Сервис доставки здоровой еды

## Схема БД

![image](https://user-images.githubusercontent.com/19695435/144130192-584ee63c-9b45-4869-bdb0-9a021e3bf9c5.png)


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
