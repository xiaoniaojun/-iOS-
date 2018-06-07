# LSN2 MVC

#### struct和class的区别

其中两个区别是：struct类型不能继承；struct类型传值时传递的是它的拷贝，包括赋值，加入集合类型中等等。
（有写时拷贝等优化）

数组、字典、String、Int、UInt32这些都是struct类型。

#### 语法糖:字典

```swift
var emoji = [Int:String]()
```

#### optional类型的判别

```swift
emoji[card.identifier] ?? "?"
```
如果emoji[card.identifier]为nil，则返回"?"

#### 类型转换需要使用构造器

```swift
UInt32(intVal)
```

#### 随机函数

```swift
arc4random_uniform(UInt32(emojiChoises.count))
```

#### 语法糖：if

嵌套的if语句
```swift
if () {
    if () {
        ...
    }
}
```
可以写成：
```swift
if () , () {

}
```