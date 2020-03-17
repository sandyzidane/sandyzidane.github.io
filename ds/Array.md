# 数组

## 能力

下标定位

增加元素

删除元素

遍历

## 代码

下标访问

```java
int[] intArr = new int[]{99, 88, 77, 66, 55};
System.out.println(intArr[0]);
```

获取长度

```java
System.out.println(intArr.length);
```

遍历

```java
for (int i = 0; i < intArr.length; i++) {
		System.out.println(String.format("index: %s, value: %s", i, intArr[i]));
}
```

clone

```java
int[] copyIntArr = intArr.clone();
System.out.println(copyIntArr.length);
```

