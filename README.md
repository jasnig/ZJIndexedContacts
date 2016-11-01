# ZJIndexedContacts
一个常用的带索引的联系人列表, 同时已经处理好了联系人按拼音排序分组, 已经处理好了联系人按拼音首字母搜索的功能

![contacts.gif](http://upload-images.jianshu.io/upload_images/1271831-f63b2c4e28f53b1e.gif?imageMogr2/auto-orient/strip)


```
 NSArray *testArray = @[@"ZeroJ", @"曾晶", @"你好", @"曾晶", @"曾晶" , @"曾晶" , @"曾晶" , @"曾晶" , @"曾晶" , @"曾晶" , @"曾晶",  @"曾好", @"李涵", @"王丹", @"良好", @"124"];
    
    NSMutableArray<ZJContact *> *contacts = [NSMutableArray arrayWithCapacity:testArray.count];
    for (NSString *name in testArray) {
        ZJContact *test = [ZJContact new];
        test.name = name;
        test.icon = [UIImage imageNamed:@"icon"];
        [contacts addObject:test];
    }

    [self setupInitialAllDataArrayWithContacts:contacts];
```