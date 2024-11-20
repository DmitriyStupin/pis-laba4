# Лабораторная работа №4 по ПИС
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
