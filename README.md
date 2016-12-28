# NotesOfObjective-C

##### `dynamic`: 告诉不让编译器在编译时自动生产 accessors，比如在子类化 NSManagedObject 时候告诉编译器会在运行时创建。
##### 为什么子类化 NSManagedObject 是要使用 `dunamic`：因为 `properties` 是不是实例变量
##### `atomic`是线程安全的，默认为`atomic`，所以一般需要加 `natomic` 修饰
##### `assign`修饰纯量 CGFloat NSInteger
##### `delegate` 如果  `responseToSelector` 调用的多的话，可以使用段位结构体来缓存这个结果
