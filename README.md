```java
List<String> generics = null;
    List notGenerics = new ArrayList(10);
    notGenerics.add(new Object());
    notGenerics.add(new Integer(1));
    
    generics = notGenerics;
    // 此处抛出ClassCastException异常
    String string = generics.get(0);
```
