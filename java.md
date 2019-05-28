```java

public class TestClass<T> {}

public interface TestInterface<T> {}

class box{
  private Object box;
  public void set(Object box){ this.box = box; }
  public Object get(){ return this.box; }
}

Box box = new Box();
box.set("ABSDF");
// String -> Object
String val = (String)box.get();
// Object -> String

class box<T> {
  private T box;
  public void set(T box){ this.box = box; }
  public T get(){ return this.box; }
}

Box<String> box = new Box<String>();
// Generic T -> String 으로 변환
box.set("ABSDF");
String val = box.get();

public class Box<T, M>{
  private T box1;
  private M box2;
  
  public T getBox1(){ return this.box1; }
  public void setBox1(T box1){ this.box1 = box1; }
  
  public M getBox2(){ return this.box2; }
  public void setBox2(M box2){ this.box2 = box2; } 

}

Box<String, Integer> box = new Box<String, Integer>();
box.setBox1("AAA");
box.setBox2(14433);

```
