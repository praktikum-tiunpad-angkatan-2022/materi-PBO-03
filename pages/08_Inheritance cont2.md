# Inheritance (cont.)

<div class="grid grid-cols-2 gap-4">

<div v-click="1">

```java
/**
 * Animal.java
 */
public class Animal {
    private int legCount;

    public Animal() { this.legCount = 2; }

    public Animal(int legCount) {
        this.legCount = legCount;
    }

    protected void setLegCount(int legCount) {
        this.legCount = legCount;
    }

    protected int getLegCount() {
        return this.legCount;
    }
}
```

</div>
<div>
<div v-click="2">

```java
/**
 * Cat.java
 */
public class Cat extends Animal {
    public Cat() {
        super(4);
    }
}
```

</div>
<div v-click="3" class="mt-4">

```java
/**
 * Main.java
 */
public class Main {
    public static void main(String[] args) {
        Cat catus = new Cat();
        System.out.println(catus.getLegCount()); // 4
        catus.setLegCount(8);
        System.out.println(catus.getLegCount()); // 8
    }
}
```

</div>
</div>
</div>
