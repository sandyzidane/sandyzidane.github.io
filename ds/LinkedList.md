# 链表

## 单链表

![示意图](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2013/03/Linkedlist.png)

### 节点

```java
class Node<T> {
  T data;
  Node<T> next;
  
  public Node(T data) {
    this.data = data;
  }
}
```

### 单链表

```java
class SingleLinkedList<T> {
  Node<T> head;
}
```

### 操作

#### 创建

```java
SingleLinkedList<Integer> linkedList = new SingleLinkedList<>();
linkedList.head = new Node<>(3);
linkedList.head.next = new Node<>(2);
linkedList.head.next.next = new Node<>(1);
```

#### 遍历

```java
System.out.println("遍历链表");
Node<Integer> nextNode = linkedList.head;
while (nextNode != null) {
  System.out.println(nextNode.data);
  nextNode = nextNode.next;
}
```

#### 尾部插入

#### 头部插入

#### 查询节点



## 双链表

## 循环链表

