# 'super' Keyword (cont.)

<div class="grid grid-cols-2 gap-4">

<div>

<div v-click="1">

```java
/**
 * Animal.java
 */
public class Animal {
    public int legCount;

    public Animal() { this.legCount = 2; }
}
```

</div>
<div v-click="2" class="mt-4">

```java
/**
 * Cat.java
 */
public class Cat extends Animal {
    public int legCount = 4;
    public Cat() { super(); }

    public void info() {
        System.out.println(legCount); // 4
        System.out.println(this.legCount); // 4
        System.out.println(super.legCount); // 2
    }
}
```

</div>
</div>
<div v-click="3">

```java
/**
 * Main.java
 */
public class Main {
    public static void main(String[] args) {
        Cat catus = new Cat();
        catus.info();
    }
}
```

</div>
</div>
