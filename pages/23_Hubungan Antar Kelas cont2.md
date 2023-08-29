
# Hubungan Antar Kelas (cont.)

<br>

**Composition** merupakan hubungan antara class (entity) dengan dependency yang memiliki lifespan sama. Jika 1 class telah mati, maka dependency pun **akan ikut mati**.

<div class="flex justify-center mt-16">
<div class='w-4/5'>

```mermaid
classDiagram
    direction LR
    User *-- Address
    class User {
        -id: int
        -name: String
        -address: Address
        +User(id: int, name: String, address: Address)
    }
    class Address {
        -id: int
        -streetNumber: int
        -city: String
        +Address(id: int, streetNumber: int, city: String)
    }
```

</div>
</div>