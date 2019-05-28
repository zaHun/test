```java

public class TestClass<T> {}

public interface TestInterface<T> {}

class box{
  private Object box;
  public void set(Object box){ this.box = box; }
  public Object get(){ return this.box; }
}

class box<T> {
  private T box;
  public void set(T box){ this.box = box; }
  public T get(){ return this.box; }
}

```
