
# Method Overriding

Menulis kembali method dari superclass pada subclassnya untuk memperoleh implementasi yang lebih spesifik.

<div class="mt-4">
<div>

```java
/**
 * Animal.java
 */
class Animal {
    public void walk() {
        System.out.println(getClass().getSimpleName() + " walks!");
    }
}
```

</div>
<div>

```java
/**
 * Cat.java
 */
class Cat extends Animal {
    @Override
    public void walk() {
        super.walk();
        System.out.println("This cute " + getClass().getSimpleName() + " walks!");
    }
}
```

</div>
</div>
