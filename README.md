Задание №161
Таблица
![0_table](https://github.com/user-attachments/assets/fd310a2c-f4c7-4c59-acd7-11ee802c7b81)
Выберите из таблицы orders 3 самых дешевых заказа за всё время. Данные нужно отсортировать в порядке убывания цены. Отмененные заказы не учитывайте.
![1](https://github.com/user-attachments/assets/4352e865-833e-46d3-83f4-6284a33e28c8)
select * from orders where status in('new','in_progress','delivery') order by sum desc limit 3;
Выберите из таблицы orders 2 самых дорогих заказов за всё время. Данные нужно отсортировать в порядке убывания цены. Отмененные заказы не учитывайте.
![2](https://github.com/user-attachments/assets/e10e21d4-4bde-43fa-8b89-bca74e2ac01e)
select * from orders where status in('new','in_progress','delivery') order by sum desc limit 2;
Задание №166
Таблица
![0_table (1)](https://github.com/user-attachments/assets/ac9d3d98-b27d-45be-8346-1f57f9182205)
Добавьте в таблицу orders данные о новом заказе стоимостью 8000 рублей. В заказе 4 товара (products).\
![1 (1)](https://github.com/user-attachments/assets/e0594ad3-9628-4440-8afa-b6b102314d8b)
insert into orders (id, products, sum) value (6, 4, 8000);
![1_result](https://github.com/user-attachments/assets/6d067072-9583-47cf-9938-2cd40775ce23)
Задание №167
Таблица
![0_table (2)](https://github.com/user-attachments/assets/2d1f8486-5194-4ecd-b325-8af4be906bbe)
Добавьте в таблицу products новый товар — «VR-очки», стоимостью 70000 рублей в количестве (count) 2 штук.
![1 (2)](https://github.com/user-attachments/assets/7da02020-12ed-49f0-9730-67219b83d104)
insert into products (id, name, count, price) value (7, 'VR-очки', 2, 70000);
![1_result (1)](https://github.com/user-attachments/assets/441b0c7b-6218-4b26-a4ca-f2ab4764b05d)
Задание №172
Таблица
![0_table (3)](https://github.com/user-attachments/assets/c39129e7-1d52-44be-b6ad-130fad502931)
В таблицу products внесли данные с ошибкой, вместо "PS5" в наименовании написали IMAC. Исправьте ошибку.
![1 (3)](https://github.com/user-attachments/assets/1a88bf0f-38e1-4860-a89e-a4964cde97b5)
update products set name='PS5' where id=7;
![1_result (2)](https://github.com/user-attachments/assets/fe2cd5ce-c13d-4eec-bd03-5cf93ea817cb)
