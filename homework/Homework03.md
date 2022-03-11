# **SuppressWarnings**

## **代码演示**

```java

public class Homework03 {
    public static void main(String[] args) {
        Animal[] animals = new Animal[3];
        animals[0] = new Cat();
        animals[1] = new Cat();
        animals[2] = new Dog();
        for (Animal animal : animals) {
            if (animal instanceof Cat) {
                ((Cat) animal).shout();
            }
            if (animal instanceof Dog) {
                ((Dog) animal).shout();
            }
        }
    }
}

abstract class Animal {
    abstract void shout();
}

class Cat extends Animal {
    @Override
    void shout() {
        System.out.println("喵喵喵");
    }
}

class Dog extends Animal {
    @Override
    void shout() {
        System.out.println("汪汪汪");
    }
}


```

# 代码

# 代码回退测试
