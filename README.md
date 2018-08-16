```java
    try {
      if (com.alibaba.fasttext.sec.url.CheckSafeUrl.getDefaultInstance().inWhiteList(targetUrl)) {
            response.sendRedirect(targetUrl);
        }
    } catch (IOException e) {
        logger.error("Check returnURL error! targetURL:{}", targetURL, e);
        throw e;
    }
```
