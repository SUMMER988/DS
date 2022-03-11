# **enum 来实现枚举类**

## **代码演示枚举**

```java
public class EnumDetail {
    public static void main(String[] args) {
        Music.CLASSIC_MUSIC.playing();
    }
}

class A {

}

/*
 1.使用enum关键字后，就不能再继承其它类了，
 因为enum会隐式继承Enum，而Java是单继承机制
 enum Season3 extends A {

 }
 2.enum实现的枚举类，仍然是一个类，所以还是可以实现接口的.
*/
interface IPlaying {
    public void playing();
}

enum Music implements IPlaying {
    CLASSIC_MUSIC;
    @Override
    public void playing() {
        System.out.println("播放好听的音乐...");
    }
}

```

# 代码
