# leetcode hot 100刷题笔记

## 1

建立哈希表

```java
Map<Integer,Integer> hashtable = new HashMap<>();
//其中Integer为哈希表中键和值的数据类型的包装类，例如49题中Integer换成了如下所示
Map<String,List<String>> hashtable = new HashMap<>();
```

HashMap在1中运用了如下方法

```java
hashtable.get();//括号内输入键，会得到哈希表内键值对应的值
hashtable.put(,);//逗号前后分别放入键和值
hashtable.containsKey();//括号内输入键查找哈希表内是否存在该键，返回值为布尔类型
```

## 49

string中的方法

```java
String.toCharArray();//toCharArray() 是 String 类的一个方法，它将当前字符串中的所有字符复制到一个新的字符数组中，并返回这个字符数组。
String.valueOf();// 是一个静态方法，它可以将各种类型的原始数据类型（如 int、char、boolean 等）或者对象转换为字符串
Arrays.sort();//是一个用于对数组进行排序的方法Arrays类中的方法
```

循环访问String s{"a","avbafg","salfjl"}中各个字符串的方法

```java
for(String str : s);//依次把s中各个字符串赋给str
```

HashMap中的方法

```java
map.getorDefault(Object key, V defaultValue);//key为要查找的键值，V为Map中值的类型
```

用法示例

```java
Map<String, List<String>> map = new HashMap<>();
List<String> defaultValue = new ArrayList<>();
List<String> list = map.getOrDefault("key", defaultValue);

// 如果map中存在键"key"，则list将包含"key"对应的值。
// 如果map中不存在键"key"，则list将是传递给getOrDefault方法的defaultValue，即一个新的ArrayList实例。    
```

List接口的方法

```java
List<String> list = new ArrayList<>();
list.add("element");//将element加到list的末尾，返回值为布尔类型，表示是否添加成功
```
