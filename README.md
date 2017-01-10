# NotesOfObjective-C

`dynamic`: 告诉不让编译器在编译时自动生产 accessors，比如在子类化 NSManagedObject 时候告诉编译器会在运行时创建。
为什么子类化 NSManagedObject 是要使用 `dunamic`：因为 `properties` 是不是实例变量
`atomic`是线程安全的，默认为`atomic`，所以一般需要加 `natomic` 修饰
`assign`修饰纯量 CGFloat NSInteger
`delegate` 如果  `responseToSelector` 调用的多的话，可以使用段位结构体来缓存这个结果

dealloc
1. 一般之做比较“轻量级”的操作，比如取消 `KVO` 和通知
2. 中不要调用存取方法，因为有可能覆写这些方法导致不能被回收
3. 不要执行异步操作
