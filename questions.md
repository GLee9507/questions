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