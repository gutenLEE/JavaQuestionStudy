# 6. 클래스, 객체, 인스턴스의 차이
by gutenLEE

---

### Class
객체의 설계도 또는 틀. 객체를 생성하기 위한 필드와 메소드가 정의되어 있다. 
```java
class Car {
    String color;
    private void move(){};
}
```

## Object & Instance
자바의 정석, 자바의신, 이것이 자바다를 모두 확인해본 결과, 저자 마다 견해가 약간씩은 다르나
object 와 instance는 같은 의미라 보면 된다.

### Object
객채는 **추상적 의미**가 강함.  
객체의 정의 : 실제로 존재하는 것. 사물 또는 개념  
객체의 용도 : 객체가 가지고 있는 기능과 속성에 따라 다름.  

객체는 클래스에 정의된 대로 생성된다.
```java
Car bmw
Car audi
Car kia
```
### Instance
객체의 실체. 구체적인 메모인 메모리를 가르키고 있는 경우.  
인스턴스는 객체와 같은 의미이지만, 객체는 모든 인스턴스를 대표하는 **포괄적인 의미**를 갖고 있음.   
인스턴스는 어떤 클래스로부터 만들어진 것인지를 강조하는 **보다 구체적인 의미**를 갖고 있음.
```java
Car bmw = new Car();
Car audi = new Car();
Car kia = new Car();
```

인스턴스와 객체는 같은 의미이지만, 문맥에 따라 구별하여 사용하는 것이 좋음.
```mermaid
    flowchart LR
     Car_Class --> id(instance or object)
```
- 책상은 인스턴스다? -> 책상은 객체다.
- 책상은 책상 클래스의 객채다? -> 책상은 책상 클래스의 인스턴스다. 