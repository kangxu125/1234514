```java
Lock lock = new XxxLock();
    preDo();
    try {
            // 无论加锁是否成功，unlock都会执行
        lock.lock();
        doSomething();
    } finally {
        lock.unlock();
    }
```
