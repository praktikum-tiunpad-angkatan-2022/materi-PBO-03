
# Hubungan Antar Kelas (cont.)

<br>

**Aggregation** merupakan hubungan antara class (entity) dengan dependency yang memiliki lifespan berbeda. Jika 1 class telah mati, tetapi dependency **tidak akan ikut mati**.

<div class="flex justify-center mt-16">
<div class='w-4/5'>

```mermaid
classDiagram
    direction LR
    School o-- Student
    class School {
        -id: String
        -name: String
        -students: ArrayList<Student>
        +Student(id: String, name: String)
        +addStudent(newStudent: Student)
    }
    class Student {
        -id: String
        -name: String
        +Student(id: String, name: String)
    }
```

</div>
</div>