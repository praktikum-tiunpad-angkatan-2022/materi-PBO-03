
# Method Overriding (Other)

<div class="mt-4 grid grid-cols-2 gap-x-4">
<div>

Python

```python
class Animal:
   def walk(self):
       print(self.__name__ + " walks!")

class Cat(Animal):
   def walk(self):
       print("This cute " + self.__name__ + " walks!")
```

</div>
<div>

C++

```cpp
class Animal {
  public:
    void walk() {
      cout << "Animal walks!";
    }
};

class Cat: public Animal {
  public:
    void walk() {
      cout << "This cute cat walks!";
    }
};
```

</div>
</div>
