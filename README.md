# Soal 1

Relasi One to One

```javascript
    {
        "_id": ObjectId('12345'),
        "fullName": "Dinda Viera Nursabrina",
        "email": "dinda111@gmail.com",
        "phoneNumber": "0888888111"
    }
```

# Soal 2

Relasi : one to few

```javascript
    {
       "_id": ObjectId('12345'),
       "fullName": "Dinda Viera Nursabrina",
       "email": "dinda111@gmail.com",
       "phoneNumber": "0987167671",
       "address" : [
           {
               "street" : "Jl. Kenangan no 1",
               "city" : "Semarang"
           },
           {
               "street" : "Jl. aja dulu no 2",
               "city" : "Jakarta"
           }
       ]
   }
```

# Soal 3

Relasi : One to Many

```javascript
    {
        "_id": ObjectId('45678'),
        "productName": "Kaos Polos",
        "brandName": "SkilShirt",
        "variants": [
            {
            "variantName": "Kaos Polos Hitam",
            "color": "Hitam",
            "quantity": 12,
            "price": "Rp 99.000"
            },
            {
            "variantName": "Kaos Polos Navy",
            "color": "Navy",
            "quantity": 10,
            "price": "Rp 99.000"
            }
        ]
    }
```

# Soal 4

Relasi : Many to Many

Film Schema

```javascript
    {
        "_id": ObjectId("AAAB1"),
        "filmName": "Venom 2"
    },
    {
        "_id": ObjectId("AAAB2"),
        "filmName": "Spiderman No Way Home"
    }

```

Cinema Schema

```javascript
    {
        "_id": ObjectId('CCC1'),
        "cinemaName": "CGF",
        "location": "Pondok Indah Mall",
        "films": [
            "ObjectId('AAAB1')",
            "ObjectId('AAAB2')"
        ]
    },
    {
        "_id": ObjectId('CCC2'),
        "cinemaName": "Cinema31",
        "location": "Mall Kelapa Gading",
        "films": [
            "ObjectId('AAAB1')",
            "ObjectId('AAAB2')"
        ]
    }

```
