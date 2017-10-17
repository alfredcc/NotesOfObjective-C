#pragma 隐藏 warnings
``` Objective-C
// completionBlock在AFURLConnectionOperation中被手动的设置为nil来打破保留周期。
#pragma clang diagnostic push
#pragma clang diagnostic ignored "-Warc-retain-cycles"
    self.completionBlock = ^ {
        ...
    };
#pragma clang diagnostic pop
```

类别（Category）：增加新的类和实例方法来扩展现有类的行为。
``` Objective-C
@interface MyObject (CategoryName)
  - (void)foo;
  - (BOOL)barWithBaz:(NSInteger)baz;
@end
```

类扩展（Class Extension):通常在 @implementation 前定义来指定私有接口
