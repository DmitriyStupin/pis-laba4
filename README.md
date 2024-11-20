# Лабораторная работа №4 по ПИС
[Use-Case диаграмма UML](https://github.com/DmitriyStupin/pis-laba4/blob/main/Use-%D0%A1ase%20%D0%B4%D0%B8%D0%B0%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0%20UML.pdf){target="_blank"} <br>
[Интерфейсы и прецеденты](https://github.com/DmitriyStupin/pis-laba4/blob/main/%D0%9F%D0%98%D0%A1%20%E2%84%964%20(%D0%98%D0%BD%D1%82%D0%B5%D1%80%D1%84%D0%B5%D0%B9%D1%81%D1%8B%20%D0%B8%20%D0%BF%D1%80%D0%B5%D1%86%D0%B5%D0%B4%D0%B5%D0%BD%D1%82%D1%8B).pdf){target="_blank"}

Форматы данных:
1. Товар (Product)
```console
{
  "id": "12345",
  "name": "Яблоня",
  "type": "Декоративная",
  "price_retail": 500,
  "price_wholesale": 475,
  "quantity": 100,
  "description": "Краткое описание товара."
}
```

2. Покупатель (Customer)
```console
{
  "id": "56789",
  "name": "Иван Иванов",
  "phone": "+7 999 123 45 67",
  "cart": [
    {
      "product_id": "12345",
      "quantity": 2
    },
    {
      "product_id": "67890",
      "quantity": 1
    }
  ]
}
```

3. Заказ (Order)
```console
{
  "order_id": "ABC123",
  "customer_id": "56789",
  "items": [
    {
      "product_id": "12345",
      "quantity": 2,
      "price": 500
    },
    {
      "product_id": "67890",
      "quantity": 1,
      "price": 1000
    }
  ],
  "total_price": 2000,
  "discount": 0,
  "order_date": "2024-11-20",
  "is_wholesale": false
}
```

4. Магазин (Store)
```console
{
  "id": "1",
  "name": "Магазин №1",
  "inventory": [
    {
      "product_id": "12345",
      "quantity": 26
    },
    {
      "product_id": "67890",
      "quantity": 14
    }
  ]
}
```

5. Доставка (Delivery)
```console
{
  "delivery_id": "DEL456",
  "store_id": "1",
  "items": [
    {
      "product_id": "12345",
      "quantity": 10
    },
    {
      "product_id": "67890",
      "quantity": 5
    }
  ],
  "delivery_date": "2024-11-25",
  "status": "В пути"
}
```
