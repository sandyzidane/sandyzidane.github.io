# zookeeper curator 分布式锁

## 使用方式

### Java 7 try-with-resources 方式

```java
InterProcessMutex mutext = new InterProcessMutext(...);	//其他 InterProcessLock 的实现也可以
try (Locker locker = new Locker(mutex, maxTimeout, unit)) {
  //do work
}
```

### 自己获取锁，释放锁

```java
InterProcessMutext mutex = new InterProcessMutext(...);

try {
  mutex.aquire();
  //do work
}
finally {
  mutex.release();
}
```

