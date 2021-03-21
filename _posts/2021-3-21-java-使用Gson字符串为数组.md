---

layout: post 
title:  json str -> List 
date: 2021-03-21 
tags: java,json

---

##  java处理 形如“[[1,2,3],[1,2,3]]”字符串为数组

```java
Gson gson = new Gson();
String str  = "[[1,3,5, 4],[1,3,5, 4]]";
List persons = gson.fromJson(str, new TypeToken<List<List<Integer>>>(){}.getType());
System.out.println(persons);
```

将  **TypeToken**\<T>中的类型与需要解码的字符串一一对应即可



## 测试一下标题

