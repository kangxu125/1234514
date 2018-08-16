```java
objectThreadLocal.set(someObject);
    try {
        ...
    } finally {
        objectThreadLocal.remove();
    }
```
