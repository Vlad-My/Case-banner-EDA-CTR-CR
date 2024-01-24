# Case-banner-EDA-CTR-CR
## 1) Легенда
Мы - онлайн магазин спортивных товаров: одежды, обуви, аксессуаров и спорт-питания. На главной странице магазина мы показываем пользователям баннеры с целью стимулирования своих продаж. Сейчас там случайно показывается один из 5 баннеров. Каждый баннер рекламирует конкретный продукт или всю компанию. Наши маркетологи считают, что:
опыт взаимодействия с баннерами может различаться по сегментам, а их эффективность – зависеть от особенностей пользовательского поведения.
У менеджера компании появилось предложение от партнеров продать это место для баннера и рекламировать там другой сервис (оплата предполагается по CPC-модели, т.е. стоимость за клик).

## 2) Задача
Помочь менеджеру принять решение – нужно ли продавать это место для рекламы другого сервиса.

## 3) Стек
- Python:
  - pandas
  - seaborn
  - numpy
  - pingouin
  - matplotlib.pyplot
## 4) Этапы
1) Проводим EDA (Exploratory Data Analysis)
2) Подготавливаем данные
3) Рассчитаем CTR % (кликабельность объявлений) и CR % (коэффициент конверсии в заказы)
## 5) Выводы
Для принятия взвешенного решения продать место для баннера или использовать самим нужно больше данных, как минимум - цена за клик от пратнёров и данные по сумме наших продаж с конверсий от этих баннеров сейчас.
Но, основываясь на имеющихся данных, в целом видно, что баннеры работают неплохо, CTR находится выше среднего уровня по сравнению с рыночным бенчмарком. CR пережил два спада, и в последнее время корректируется. С февраля по май CR находился на среднерыночном уровне. Benchmarks:
https://www.wordstream.com/blog/ws/2023/05/15/google-ads-benchmarks
Для сравнения можно взятьк атегории:
Shopping, Collectibles & Gifts (CTR: 6.39%, CR: 3.69%)
Sports & Recreation (CTR: 10.53%, CR: 5.69%)

- Баннеры категории "company" не конвертируются в заказы - необходимо доп. исследование несут ли такие баннеры имиджевую ценность.
- Возможно от company стоит отказаться в пользу показа баннеров продуктов или обсудить опцию продажи показов баннеров партнёров в этом слоте.
- На первом месте по CTR и CR находятся баннеры из категории "clothes" 18% и 9,5% соответственно
- Самый низкий CR у "sports_nutrition" 2%
- Важно обратить внимание PM-а, что в десктопной версии CTR в 3 раза ниже, чем в мобильной, при этом конверсия в заказ в 2 раза выше
