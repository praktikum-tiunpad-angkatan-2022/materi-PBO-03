---
layout: center
---

# Inheritance (cont.)

<div class="grid grid-cols-2 gap-y-10 gap-x-2 mt-8">
<div class='flex-row'>

```mermaid
classDiagram
    Hewan <|-- Karnivora
    Hewan <|-- Herbivora
    Karnivora <|-- Harimau
    Karnivora <|-- Elang
    Herbivora <|-- Kambing
```

</div>
<div class='flex-row flex justify-center items-center'>
<div class='text-base text-justify mt-4'>

- Java hanya mengizinkan **single inheritance**, yakni _subclass_ hanya dapat memiliki **satu** _parent class_.

- Satu _parent class_ dapat memiliki **banyak** _subclass_ yang disebut **hierarchical inheritance**.

- Satu _subclass_ dapat memiliki _subclass_ lagi, disebut **multilevel inheritance**.

- Java tidak mendukung multiple inheritance, yakni satu _subclass_ memiliki **lebih dari satu** _parent class_.

</div>
</div>
</div>
