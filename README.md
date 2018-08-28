```java
public class ConfusingName {
        public int alibaba;
        // 非setter/getter的参数名称，不允许与本类成员变量同名
        public void get(String alibaba) {
            if(true) {
            final int taobao = 15;
                // ...
            }
    
            for (int i = 0; i < 10; i++) {
                // 在同一方法体中，不允许与其它代码块中的taobao命名相同
                final int taobao = 15;
                // ...
            }
        }
    }

    class Son extends ConfusingName {
        // 不允许与父类的成员变量名称相同
        public int alibaba;
    }
```
