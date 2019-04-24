## 1. LeakCanary 是如何检测内存泄漏的
在 Activity/Fragment（简称A/F）创建时 LeakCanary 弱引用持有 A/F 并注册监听 A/F 生命周期，在其生命周期结束时调用系统函数 Runtime.getRuntime().gc() 触发 GC 。等待些许时间后判断弱引用的 A/F 是否可达，如果可达证明其发生内存泄漏。

## 2. BlockCanary 是如何检测主线程卡顿的


## 3. Java 内存模型
### 1. 什么是内存模型
### 2. 什么是 Java 内存模型

## 4. HashMap 原理 1.7&1.8
HashMap 是一种以键值对


## 5. ConcurrentHashMap 原理 1.7&1.8

## 6. ArrayMap SparseArray

## 7. Activity 跳转生命周期

当由Activity A跳转到Activity B时的执行顺序

A 的 onPause() > B 的 onCreate() > B 的 onStart() > B 的 onResume() > A 的 onStop()


当按返回按钮由Activity B返回到Activity A时的执行顺序

B 的 onPause() > A 的 onRestart() > A 的 onStart() > A 的 onResume() > B 的 onStop() > B 的 onDestroy()







Retrofit 动态代理细节，为什么要用 Retrofit

Java 内存模型，volatile 关键字

计算机内存为什么要分为堆和栈

java 线程安全，生产者消费者模型

HTTP/HTTPS 

TCP/UDP 如何设计一个可靠地UDP协议

Rxjava2 中的 Flowable 和 Observable 区别，什么是背压

Kotlin 与 java 泛型

什么是死锁，如何解决

红黑树原理，时间复杂度

HashMap HashTable ConcurrentHasMap 1.7/1.8 原理

RecyclerView 与 ListView 的区别

主线程 Looper 一直在循环阻塞但页面为什么不会卡顿

计算 ViewGroup 中的所有子 View 数量

View 的 onMeasure onLayout onDraw 流程，自定义View ViewGroup

事件分发流程，如何解决滑动冲突

什么是 CAS，原理 缺点 。什么是 ABA 问题，如何解决

Activity 启动模式以及应用

二叉树 前、中、后 序遍历，之字形层序遍历

校验二叉搜索树

类加载机制，双亲委派模型

APK 打包流程，签名算法

性能优化

ANR 原理，解决

爬楼梯问题，动态规划






































