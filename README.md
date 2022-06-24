# Домашнее задание к занятию «2.3. Patterns»

## Задача №1 - Заказ доставки карты (изменение даты)

Вам необходимо автоматизировать тестирование новой функции формы заказа доставки карты:

![](pic/order.png)

Требования к содержимому полей, сообщения и другие элементы, по словам Заказчика и Разработчиков, "такие же, мы ничего не меняли"*.

Примечание*: личный совет - не забудьте это перепроверить, никому нельзя верить 😈.

Тестируемая функциональность: если заполнить форму повторно теми же данными за исключением "Даты встречи", то система предложит перепланировать время встречи:

![](pic/replan.png)

После нажатия на кнопке "Перепланировать" произойдёт перепланирование встречи:

![](pic/success.png)

**Важно:** в этот раз вы не должны хардкодить данные прямо в тест! Используйте Faker, Lombok, Data-классы (для группировки нужных полей) и утилитный класс-генератор данных* - см. пример в презентации.

Утилитными называют классы, у которых приватный конструктор и статичные методы.

Обратите внимание, что Faker может генерировать не совсем в нужном для вас формате.