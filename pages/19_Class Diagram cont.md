---
layout: center
---

<div class="grid grid-cols-2 gap-y-10 gap-x-6 mt-4">
<div class='flex items-center'>

<div>

# Class Diagram (cont.)

</div>
</div>
<div class='flex-row flex justify-center items-center'>

```mermaid
classDiagram
    class Student {
        -name: String
        -age: int
        -studentId: String
        +Student(name: String)
        +Student(name: String, age: int, studentId: String)
        +setName(name: String)
        +setStudentId(studentId: String)
        +getName() String
        +printStudent()
    }
```

</div>
</div>