# Flutter学(cai)习(keng)之路

坑の顺位: ↓

1. Waiting for another flutter command to release the startup lock...

- 删除SDK中的flutter/bin/cache/lockfile文件

2. [pubspec.yaml修改后点击packages get后长时间无反应，提示: Running "flutter pub get" in flutter_app](https://blog.csdn.net/unique_Even/article/details/104995111)

3. XXX called with a context that does not contain a Scaffold

- 注意要在State中的body节点对应new一个Builder，且通过命名参数显式的传递一个上下文参数，否则就会报如上错误。

- 具体写法可参照代码: [https://stackoverflow.com/questions/51304568/scaffold-of-called-with-a-context-that-does-not-contain-a-scaffold](https://stackoverflow.com/questions/51304568/scaffold-of-called-with-a-context-that-does-not-contain-a-scaffold)
