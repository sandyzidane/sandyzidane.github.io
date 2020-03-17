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

#### 头部插入

```java
public void insertFirst(T newData) {
  Node<T> newNode = new Node<>(newData);
  
  Node<T> h = head;
  head = newNode;
  newNode.next = h;
}
```



#### 尾部插入

```java
public void insertLast(T newData) {
  Node<T> newNode = new Node<>(newData);
  
  //特殊处理
  if (head == null) {
    head = newNode;
    return;
  }
  
  //遍历到最后一个节点
  Node<T> nextNode = head;
  while (nextNode.next != null) {
    nextNode = nextNode.next;
  }
  nextNode.next = newNode;
}
```



#### 指定位置插入

#### 查询节点



## 双链表

## 循环链表

