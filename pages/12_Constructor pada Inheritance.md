---
layout: center
---

# Constructor pada Inheritance

<div class="grid grid-cols-2 gap-y-10 gap-x-6 mt-4">
<div class='flex-row'>
<div class='text-base text-justify mt-4'>

- Hanya member class _properties_ dan _methods_ yang diwariskan, **konstruktor tidak diwariskan**.

- Ketika object child dibuat (konstruktornya dieksekusi), maka konstruktor parent class dijalankan terlebih dahulu kemudian menyelesaikan konstruktor child.

> 1. Coba compile class Cat di samping, apa yang terjadi?
>
> 2. Kemudian pindahkan super() sebelum `this.legCount = 8`
> pada class Cat di samping, compile ulang, dan lihat apa
> yang terjadi.

</div>
</div>
<div>
<div>

```java
/**
 * Animal.java
 */
public class Animal { }
```

</div>
<div>

```java
/**
 * Cat.java
 */
public class Cat extends Animal {
    private int legCount = 4;
    public Cat() {
        this.legCount = 8;
        super();
    }

    public void info() {
        System.out.println(legCount);
    }
}
```

</div>
</div>
</div>
