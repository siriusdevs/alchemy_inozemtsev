## Создать модели на sqalchemy, применить их к базе данных, продемонстрировать создание, выборку и удаление объектов, а также работу связи (добавление продукта к категории).

### __Категория__
*Обязательные поля:*
- id uuid PK с генерируемым значением по умолчанию
- название str (len <= 50) уникальное

*Необязательные:*
- описание str (len <= 500)
- создано datetime (по умолчанию текущее время и дата)

### __Продукт__
*Обязательные поля:*
- id uuid PK с генерируемым значением по умолчанию
- название str (len <= 30)
- price float (> 0)

*Необязательные:*
- описание str (len <= 500)
- срок годности date
- категория (связь один ко многим, внешний ключ на категорию, обязательная связь)
- создано datetime (по умолчанию текущее время и дата)
