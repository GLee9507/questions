## 1. LeakCanary 是如何检测内存泄漏的
在 Activity/Fragment（简称A/F）创建时 LeakCanary 弱引用持有 A/F 并注册监听 A/F 生命周期，在其生命周期结束时调用系统函数 Runtime.getRuntime().gc() 触发 GC 。等待些许时间后判断弱引用的 A/F 是否可达，如果可达证明其发生内存泄漏。

## 2. BlockCanary 是如何检测主线程卡顿的

