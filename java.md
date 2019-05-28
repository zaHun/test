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

```
