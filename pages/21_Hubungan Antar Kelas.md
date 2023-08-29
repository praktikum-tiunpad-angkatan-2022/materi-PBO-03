
# Hubungan Antar Kelas

<br>

**Inheritance/ Pewarisan** yakni membuat sebuah subclass dari class yang sudah ada. Hubungan ini disebut juga hubungan _spesialisasi_ dan berkebalikan dengan hubungan _generalisasi_.

<div class="flex justify-center">
<div class='w-5/6'>

```mermaid
classDiagram
    Product <|-- Furnitures
    Product <|-- Consumables
    class Product {
        #id: int
        #name: String
        #price: int
        +Product(id: int, name: String, price: int)
    }
    class Furnitures {
        -productionDate: Date
        +Furnitures(id: int, name: String, price: int, productionDate: Date)
    }
    class Consumables {
        -expirationDate: Date
        +Consumables(id: int, name: String, price: int, productionDate: Date)
    }
```

</div>
</div>